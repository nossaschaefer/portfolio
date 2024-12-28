<template>
  <header class="fixed top-0 left-0 right-0 p-4 z-50 w-full bg-[#fbf6f3] pb-2">
    <nav class="flex justify-between items-center w-full max-w-screen-3xl mx-auto sm:justify-end">
      <button @click="toggleMenu" class="block sm:hidden p-2 focus:outline-none ml-auto">
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"
          ></path>
        </svg>
      </button>
      <ul
        :class="{ block: isMenuOpen, hidden: !isMenuOpen, 'sm:flex': true }"
        class="flex flex-col sm:flex-row sm:items-center sm:gap-10 sm:static absolute top-16 right-0 bg-[#fbf6f3] sm:bg-transparent w-full sm:w-auto sm:shadow-none p-4 sm:p-0"
      >
        <li class="text-center sm:text-right">
          <a href="/home" @click.prevent="scrollToSection('home')" class="block py-2 sm:py-0"
            >Home</a
          >
        </li>
        <li class="text-center sm:text-right">
          <a
            href="/projects"
            @click.prevent="scrollToSection('projects')"
            class="block py-2 sm:py-0"
            >Projects</a
          >
        </li>
        <li class="text-center sm:text-right">
          <a href="/about" @click.prevent="scrollToSection('about')" class="block py-2 sm:py-0"
            >About</a
          >
        </li>
        <li class="text-center sm:text-right">
          <a href="/contact" @click.prevent="scrollToSection('contact')" class="block py-2 sm:py-0"
            >Contact</a
          >
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      isMenuOpen: false,
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen
    },
    scrollToSection(sectionId) {
      const section = document.getElementById(sectionId)
      if (section) {
        section.scrollIntoView({ behavior: 'smooth' })
        history.replaceState(null, '', `/${sectionId}`)
        this.isMenuOpen = false // Close the menu after clicking a link
      }
    },
  },
}
</script>

<style scoped></style>
