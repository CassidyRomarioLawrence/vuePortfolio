<template>
  <section class="home">
    <HomePage /> 
  </section>
  <section id="about">
    <h2 class="display-2 text-center mb-3">About Myself</h2>
    <AboutPage />
  </section>
  <section id="resume">
    <h2 class="display-2 text-center mb-3">Resume</h2>
    <ResumeComponent />
  </section>
  <section id="projects">
    <h2 class="display-2 text-center mb-3">Projects</h2>
    <ProjectsComponent />
  </section>
  <section id="testimonials">
    <h2 class="display-2 text-center mb-3">Testimonials</h2>
    <TestimonialComponent />
  </section>
  <section id="contact">
    <h2 class="display-2 text-center mb-3">Contact Me</h2>
    <ContactForm />
  </section>
</template>

<script>
import HomePage from '@/components/HomePage.vue';
import AboutPage from '@/components/AboutPage.vue';
import ContactForm from '@/components/ContactForm.vue';
import ProjectsComponent from '@/components/ProjectsComponent.vue';
import TestimonialComponent from '@/components/TestimonialComponent.vue';
import ResumeComponent from '@/components/ResumeComponent.vue'

export default {
  name: 'HomeView',
  components: {
    HomePage,
    AboutPage,
    ContactForm,
    ProjectsComponent,
    TestimonialComponent,
    ResumeComponent
  }
}
</script>
<style scoped>
#about,#projects{
  background-image:linear-gradient(black,rgb(100, 194, 225),black);
  min-height: 100vh;
  color: white;
  text-shadow: 3px 3px 3px black;
}
#resume,#testimonials{
  min-height: 100vh;
  color: white;
  text-shadow: 3px 3px 3px black;
}
#contact{
  background-image: linear-gradient(black, rgb(100, 194, 225), black);
  min-height: 98vh;
  color: white;
  text-shadow: 3px 3px 3px black;
}
</style>
