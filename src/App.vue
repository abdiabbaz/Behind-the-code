<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About Me</router-link> |
    <router-link to="/skills">Skills</router-link>
  </nav>
  <router-view/>
  <Sidebar />
<div :style="{ marginLeft: sidebarWidth }">

  </div>
</template>

<script>
import Sidebar from "@/components/sidebar/Sidebar.vue"
import {sidebarWidth} from "@/components/sidebar/state"
import AboutViewVue from './views/AboutView.vue'

export default {
  components: {Sidebar,
  AboutViewVue
  },
  setup(){
    return {sidebarWidth}
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #90969b;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #4a90e2;
}
</style>
