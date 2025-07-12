<template>
  <div>
    <Header />
    <About />
    <Experience />
    <Projects />
    <Contact />
  </div>
</template>

<script>
import Header from '../components/Header.vue'
import About from '../components/About.vue'
import Experience from '../components/Experience.vue'
import Projects from '../components/Projects.vue'
import Contact from '../components/Contact.vue'

export default {
  components: { Header, About, Experience, Projects, Contact }
}
</script>
