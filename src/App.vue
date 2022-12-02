<template>
  <div id="app">
    <HeaderBox :get="arraiNav"/>
  </div>
</template>

<script>

import HeaderBox from "./components/header/HeaderBox.vue"
export default {
  name: 'App',
  components: {
   HeaderBox,
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
        
      ]
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
