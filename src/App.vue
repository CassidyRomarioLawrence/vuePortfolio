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
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.card{
      padding-left: auto;
      padding-right: auto;
      min-height: 300px;
      margin-top: 8px;
      box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
      -webkit-transition: 0.25s box-shadow;
      transition: 0.25s box-shadow;
}
.card:focus,
.card:hover {
  box-shadow: 0 5px 11px 0 rgba(0, 0, 0, 0.18), 0 4px 15px 0 rgba(0, 0, 0, 0.15);
}
.card-img-top {
  padding: 20px;
  margin: auto;
}
.row {
  margin-left: auto;
  margin-right: auto;
  padding: 20px;
}
.btn {
  padding: 5px 5px;
  border: none;
  outline: none;
  color: #FFF;
  font-family: inherit;
  font-weight: 500;
  font-size: 17px;
  cursor: pointer;
  position: relative;
  z-index: 0;
  border-radius: 12px;
  margin: 8px 0;
}
.btn::after {
  content: "";
  z-index: -1;
  position: absolute;
  width: 100%;
  height: 100%;
  background-color: rgb(46, 46, 46);
  left: 0;
  top: 0;
  border-radius: 10px;
}
.btn::before {
  content: "";
  background: linear-gradient(45deg,
  #FF0000, #002BFF, #FF00C8, #002BFF,
  #FF0000, #002BFF, #FF00C8, #002BFF);
  position: absolute;
  top: -2px;
  left: -2px;
  background-size: 600%;
  z-index: -1;
  width: calc(100% + 4px);
  height: calc(100% + 4px);
  filter: blur(8px);
  animation: glowing 20s linear infinite;
  transition: opacity .3s ease-in-out;
  border-radius: 10px;
  opacity: 0;
}

.btn:hover::before {
   opacity: 1;
 }

.btn:active:after {
   background: transparent;
 }

.btn:active {
   color: #000;
   font-weight: bold;
 }

@keyframes glowing {
   0% {
     background-position: 0 0;
   }

   50% {
     background-position: 400% 0;
   }

   100% {
     background-position: 0 0;
   }
 }

 @media screen and (max-width: 360px) {
  #about p,
  #resume table,
  #projects,
  #testimonials,
  #contact input,label,button,
  .socials
   {
    font-size: 13px;
  }
  #about .my-image{
    width: 18rem;
  }
}
@media screen and (min-width: 360px) {
  #about p,
  #resume table,
  #projects,
  #testimonials,
  #contact input,label,button,
  .socials
   {
    font-size: 15px;
  }
  #about .my-image{
    width: 18rem;
  }
}
@media screen and (min-width: 1080px) {
  #about p,
  #resume table,
  #projects,
  #testimonials,
  #contact input,label,button,
  .socials
   {
    font-size: 18px;
  }
  #about .my-image{
    width: 25rem;
  }
}
</style>
