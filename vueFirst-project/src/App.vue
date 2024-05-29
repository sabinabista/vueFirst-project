 <script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from './views/FooterIndex.vue'
import AxiosWorld from './components/AxiosWorld.vue';
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
   <!-- <header> -->
      <!-- <nav class="navbar">   -->
        <!-- <nav class="bg-white px-6 flex row justify-between items-center">
        <div class="navigation">
          <img
            src="@/assets/logo.png"
            alt="logo"
            height="40px"
            width="100px"
          /> -->
        <!-- </div>
        <ul class="list">
          <ul class="flex row gap-x-5"></ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
          <li><RouterLink to="/contact">Contact</RouterLink></li> 
        </ul> 
        <ul class="flex row gap-x-5">
          <li><a href="#">Home</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">About</a></li>
        </ul>
      </nav> -->
    <!-- </header> -->

  <header>
      <nav class="bg-red-200 px-6 flex row justify-between items-center">
        <div class="navigation">
          <img
            src="@/assets/logo.png"
            alt="logo"
            height="40px"
            width="100px"
          />
        </div>
        <ul class="flex row gap-x-5">
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/about">About</RouterLink></li>
          <li><RouterLink to="/contact">Contact</RouterLink></li> 
        </ul>
      </nav>
      
    </header>

  <RouterView />
  <AxiosWorld />
  <Footer />
</template>

<style scoped>


</style> 
