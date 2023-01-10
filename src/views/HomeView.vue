<template>
  <section class="home">
    <HomePage /> 
  </section>
  <section id="about">
    <AboutPage />
  </section>
</template>

<script>
// @ is an alias to /src
import HomePage from '@/components/HomePage.vue';
import AboutPage from '@/components/AboutPage.vue'

export default {
  name: 'HomeView',
  components: {
    HomePage,
    AboutPage
  }
}
</script>
