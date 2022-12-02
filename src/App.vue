<template>
  <div id="app">
    <HeaderComp :info="headerLinks"/>
    <MainComp/>
    
  </div>
</template>

<script>

import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
  },

  data(){
    return{
      headerLinks:[
        {
          name: 'HOME',
          href: '#'
        },
        {
          name: 'ABOUT',
          href: '#'
        },
        {
          name: 'PROJECTS',
          href: '#'
        },
        {
          name: 'PROCESS',
          href: '#'
        },
        {
          name: 'TESTIMONIALS',
          href: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

</style>
