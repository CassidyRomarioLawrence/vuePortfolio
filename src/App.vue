<template>
  <NavBar />
  <FooterComponent/>
</template>
<script>
import NavBar from '@/components/NavBar.vue';
import FooterComponent from '@/components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    FooterComponent
  }
}
</script>
<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css");

#app{
  background-image: url(https://i.postimg.cc/cHpscR7Z/pexels-jaime-reimer-2662116.jpg);
    min-height: 100vh;
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
    font-family: 'Fjalla One', sans-serif;
}
</style>
