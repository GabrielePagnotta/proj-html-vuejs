<template>
    <div class="header flex">
<div>
    <img class="logo" src="../../assets/img/avada-music-logo.png" alt="">
</div>
<input id="toggle" type="checkbox">

<label for="toggle" class="hamburger">
  <div class="top-bun"></div>
  <div class="meat"></div>
  <div class="bottom-bun"></div>
</label>

<div class="nav">
  <div class="nav-wrapper">
    <nav>
        <ul>
            <li v-for="(got,index) in got" :key="index">
                <a :class="got.class" :href="got.link">{{got.name}}</a>
            </li>
        </ul>
    </nav>
  </div>
</div>
    </div>
</template>

<script>
export default {
    name: "ContentHeader",
    props:{
        got:Array,
    },
    Data(){
            return{
                got:Object
                
        }
}
}
</script>

<style lang="scss" scoped>
h1 {
  text-align: center;
  letter-spacing: 1px;
  word-spacing: 0.15em;
  font-size: 3em;
  line-height: 1.2;
  transform: translateY(52%);
}

.logo{
    margin:10%;
}

#toggle {
  display: none;
}

/**
  Hamburger
**/
.hamburger {
  position: absolute;
  top: 5em;
  right: 5%;
  margin-left: -2em;
  margin-top: -45px;
  width: 2em;
  height: 45px;
  z-index: 5;
}

.hamburger div {
  position: relative;
  width: 3em;
  height: 7px;
  border-radius: 3px;
  background-color: white;
  margin-top: 8px;
  transition: all 0.3s ease-in-out;
}

/**
Nav Styles
**/
.nav {
  position: fixed;
  width: 100%;
  height: 100%;
  background-color: #ea4a56;;
  top: -100%; left: 0; right: 0; bottom: 0;
  overflow: hidden;
  transition: all 0.3s ease-in-out;
  transform: scale(0);
}
.nav-wrapper {
  position: relative;
  overflow: hidden;
  overflow-y: auto;
  height: 100%;
}

.pink{
    color:pink;
    opacity: 80%;
}
.flex{
    display: flex;
}
nav {
  text-align: left;
  text-align: center;
}
nav a {
  position: relative;
  text-decoration: none;
  font-size: 2.3em;
  display: inline-block;
  margin-top: 2.5em;
  transition: color 0.2s ease-in-out;
  letter-spacing: 1px;
}
nav a:before {
  content: '';
  height: 0;
  position: absolute;
  width: 0.25em;
  background-color: white;
  left: -0.5em;
  transition: all 0.2s ease-in-out;
}
nav a:hover {
  color: white;
}
nav a:hover:before {
  height: 100%;
}

/**
Animations
**/
#toggle:checked + .hamburger .top-bun {
  transform: rotate(-45deg);
  margin-top: 25px;
}
#toggle:checked + .hamburger .bottom-bun {
  opacity: 0;
  transform: rotate(45deg);
}
#toggle:checked + .hamburger .meat {
  transform: rotate(45deg);
  margin-top: -7px;
}

#toggle:checked + .hamburger + .nav {
  top: 0;
  transform: scale(1);
}
</style>