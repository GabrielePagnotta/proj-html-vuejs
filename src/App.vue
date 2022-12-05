<template>
  <div id="app">
    <!-- Header -->
    <HeaderBox :get="arraiNav"/>
    <!-- Main -->
    <MusicIsLife />
    <DefaultTitle1 />
    <GridContent />
    <LastestNews />
    <CitationSinger />
    <CitationBox />
    <DefaultTitle2 />
    <ViewAllDates />
    <FooterOne :img="imgFooter"  :get="arraiFooter"/>
  </div>
</template>

<script>

import HeaderBox from "./components/header/HeaderBox.vue"
import MusicIsLife from "./components/main/MusicIsLife.vue"
import DefaultTitle1 from "./components/main/DefaultTitle1.vue"
import LastestNews from "./components/main/LastestNews.vue"
import GridContent from "./components/main/GridContent.vue"
import CitationBox from "./components/main/CitationBox.vue"
import DefaultTitle2 from "./components/main/DefaultTitle2.vue"
import ViewAllDates from "./components/main/ViewAllDates.vue"
import FooterOne from "./components/footer/FooterOne.vue"

export default {
  name: 'App',
  components: {
   HeaderBox,
   MusicIsLife,
   DefaultTitle1,
   LastestNews,
   GridContent,
   CitationBox,
   DefaultTitle2,
   ViewAllDates,
   FooterOne,
  },
  
  data(){
    return{
      arraiNav:[
        {
          name:"Home", class:"pink", link:"#"
        },
        {
          name:"Meet The Band", class:"pink", link:"#"
        },
        {
          name:"Live dates", class:"pink", link:"#"
        },
        {
          name:"Lastest News", class:"pink", link:"#"
        },
        {
          name:"Albums", class:"pink", link:"#"
        },
        {
          name:"Fans", class:"pink", link:"#"
        },
        
      ],
      
      arraiFooter:[
        {name:"Home", link:"#"},
        {name:"Meet The Band", link:"#"},
        {name:"Live Dates", link:"#"},
        {name:"Lastest News", link:"#"},
        {name:"Albums", link:"#"},
        {name:"Fans", link:"#"},
      ],

      
    }
  }
}
</script>

<style lang="scss">
*{
  margin:0;
  padding:0;
  box-sizing: border-box;
  list-style: none;
}


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}
</style>
