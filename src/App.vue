<template>
  <div class="min-h-screen bg-slate-100 text-slate-800 font-sans">
    <div class="flex flex-col lg:flex-row max-w-screen-xl mx-auto">

      <!-- Sidebar Navigation -->
      <aside
        class="lg:w-64 bg-white shadow-lg border-r border-slate-200 px-6 py-8 sticky top-0 h-screen hidden lg:flex flex-col justify-between">
        <div>
          <h1 class="text-2xl font-bold text-blue-600 mb-6">Waleed Ishag</h1>
          <nav class="space-y-4 text-sm font-medium">
            <a href="#about" class="block text-slate-700 hover:text-blue-600">About</a>
            <a href="#skills" class="block text-slate-700 hover:text-blue-600">Skills</a>
            <a href="#experience" class="block text-slate-700 hover:text-blue-600">Experience</a>
            <a href="#education" class="block text-slate-700 hover:text-blue-600">Education</a>
            <a href="#projects" class="block text-slate-700 hover:text-blue-600">Projects</a>
            <a href="#contact" class="block text-slate-700 hover:text-blue-600">Contact</a>
          </nav>
        </div>
        <footer class="text-xs text-slate-400 mt-10">© 2025 Waleed Ishag</footer>
      </aside>

      <!-- Main Content -->
      <main class="flex-1 px-6 py-10 space-y-16">
        <Hero />
        <About />
        <Skills />
        <Experience />
        <Education />
        <Projects />
        <Contact />
      </main>

    </div>
  </div>
</template>

<script>
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Experience from './components/Experience.vue'
import Education from './components/Education.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Hero,
    About,
    Skills,
    Experience,
    Education,
    Projects,
    Contact
  }
}
</script>
