<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Header from './components/Header.vue'
import Navigation from './components/Navigation.vue'
import Footer from './components/Footer.vue'
import Copyright from './components/Copyright.vue'
</script>

<template>
  <div class="app">
    <Header />
    <Navigation />
    <TopStory />
    <router-view />
    <Footer />
    <Copyright />
  </div>
</template>

<style>
@import 'material-icons/iconfont/material-icons.css';

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
}

.container {
  width: 80%;
  margin: 0 auto;
}

a {
  text-decoration: none;
  color: #000;
}

</style>
