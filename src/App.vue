<template>
  <Appbar/>
 <component :is="currentView" />
 </template>

<script>
import Appbar from './components/Appbar.vue'
import HomeView from './components/home/HomeView.vue';
import StaffDir from './components/home/StaffDir.vue';
const routes = {
  '/':HomeView,
  '/staff': StaffDir,

}

export default {
  name: 'App',
  components: {
   Appbar,
   HomeView,
  },

  data() {
    return {
      currentPath: window.location.hash
    }
  },
  computed: {
    currentView() {
      return routes[this.currentPath.slice(1) || '/'] 
    }
  },
  mounted() {
    window.addEventListener('hashchange', () => {this.currentPath = window.location.hash})
  }




}



</script>

<style >
#app{
  margin: 0px;
  background-color: whitesmoke;
  height: 100vh;
  overflow-y: hidden;
  font-family:  sans-serif;
}
</style>
>