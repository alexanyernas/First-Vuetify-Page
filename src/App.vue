<template>
  <v-app>
    <NavBar />
    <v-main>
     <HeroImage />
     <About />
     <Portfolio />
     <Project />
     <Gallery />
     <Contact />
     <Footer />
    </v-main>
  </v-app>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroImage from './components/HeroImage.vue'
import About from './components/About.vue'
import Portfolio from './components/Portfolio.vue'
import Project from './components/Project.vue'
import Gallery from './components/Gallery.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroImage,
    About,
    Portfolio,
    Project,
    Gallery,
    Contact,
    Footer
  }
};
</script>
