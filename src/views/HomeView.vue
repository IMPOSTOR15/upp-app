<template>
  
  <div class="home">
    <Navbar/>
    <HomeComponent/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeComponent from '@/components/MainPage/HomeComponent.vue'
import Navbar from '@/components/NavbarComponent.vue'
import Footer from '@/components/FooterComponent.vue'
export default {
  name: 'HomeView',
  components: {
    HomeComponent,
    Navbar,
    Footer
  }
}
</script>

<style scoped>

.home {
  /* max-width: 79vw; */
  margin: 0 auto;
}

</style>