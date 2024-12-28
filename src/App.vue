<template>
  <div>
    <HeaderComponent />
    <section id="home">
      <HomeView />
    </section>
    <section id="projects">
      <ProjectsView />
    </section>
    <section id="about">
      <AboutView />
    </section>
    <section id="contact">
      <ContactView />
    </section>
    <section id="imprint">
      <ImprintView />
    </section>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import HomeView from './views/HomeView.vue'
import ProjectsView from './views/ProjectsView.vue'
import AboutView from './views/AboutView.vue'
import ContactView from './views/ContactView.vue'
import ImprintView from './views/ImprintView.vue'

export default {
  components: {
    HeaderComponent,
    HomeView,
    ProjectsView,
    AboutView,
    ContactView,
    ImprintView,
  },
  mounted() {
    // Check if there is a hash in the URL and scroll to that section
    if (window.location.hash) {
      this.scrollToHash(window.location.hash)
    }

    // Add event listener for handling manual scrolls via hash
    window.addEventListener('hashchange', () => {
      this.scrollToHash(window.location.hash)
    })
  },
  methods: {
    scrollToHash(hash) {
      const element = document.querySelector(hash)
      if (element) {
        element.scrollIntoView({
          behavior: 'smooth',
        })
      }
    },
  },
}
</script>

<style>
html {
  scroll-behavior: smooth;
  background-color: #fbf6f3;
  width: 100%;
}
body {
  overflow-x: hidden;
}
</style>
