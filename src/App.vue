<template>
  <div>
    <NavigationBar />
    <RouterView></RouterView>
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer.vue';
import NavigationBar from './components/NavigationBar.vue';
  export default {
    name:'App',
    components: {NavigationBar, Footer}
    
  }
</script>