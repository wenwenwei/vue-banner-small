<template>
  <div id="app">
    <Banner :banners="banners"></Banner>
  </div>
</template>

<script>
import Banner from './lib/Banner'

export default {
  name: 'app',
  components: {
    Banner
  },
  data () {
    return {
      banners: {
        data: [
          {
            src: require('./assets/1.jpg'),
            url: '#1'
          },
          {
            src:  require('./assets/2.jpg'),
            url: '#2'
          },
          {
            src:  require('./assets/3.jpg'),
            url: '#3'
          },
          {
            src:  require('./assets/4.jpg'),
            url: '#4'
          }
        ],
        interval: 3000,
        target: '_blank',
        width:"900px",
        height:"500px",
        name: 'fade'
      }
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
