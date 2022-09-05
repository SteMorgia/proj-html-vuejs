<template>
  <div id="app">
    <MyHeader :siteLinks="siteLinks" />
    <MyBody />
  </div>
</template>

<script>
  import MyHeader from './components/MyHeader.vue';
  import MyBody from './components/MyBody.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyBody
  },
  data() {
    return {
      siteLinks: ['Home', 'Meet The Band', 'Live Dates', 'Latest News', 'Albums', 'Fans']
    }
  }
  

    
}
</script>

<style lang="scss">
  @import '~@fortawesome/fontawesome-free/css/all.css';
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
  }
</style>
