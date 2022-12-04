<template>
  <div id="app">
    <HeaderComp :info="headerLinks"/>
    <MainComp :cards="cardsInfo"/>
    <FooterComp/>
  </div>
</template>

<script>

import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
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
      ],

      cardsInfo:[
        {
          imgPath: 'project-1.jpg',
          text: 'Academic professional program in social media',
          category: 'social'
        },
        {
          imgPath: 'project-2.jpg',
          text: "President's speech at the annual meeting",
          category: 'institutional'
        },
        {
          imgPath: 'project-3.jpg',
          text: 'International business trip in Shangai',
          category: 'events'
        },
        {
          imgPath: 'project-4.jpg',
          text: 'Technology workshop with education theme',
          category: 'technology'
        },
        {
          imgPath: 'project-5.jpg',
          text: 'Donation of chlothes on foot to the partner NGO',
          category: 'events'
        },
        {
          imgPath: 'project-6.jpg',
          text: 'Confratenization of the procurement team',
          category: 'institutional'
        }

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
