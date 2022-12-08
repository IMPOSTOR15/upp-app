<template>
  
  <div class="home">
    <Navbar/>
    <HomeComponent/>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeComponent from '@/components/HomeComponent.vue'
import Navbar from '@/components/NavbarComponent.vue'

export default {
  name: 'HomeView',
  components: {
    HomeComponent,
    Navbar
  }
}
</script>

<style scoped>

.home {
  max-width: 79vw;
  margin: 0 auto;
}

</style>