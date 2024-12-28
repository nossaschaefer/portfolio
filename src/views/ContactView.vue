<template>
  <section
    id="contact"
    class="min-h-screen flex flex-col items-center justify-between w-full pt-20"
  >
    <div>
      <h1 class="font text-8xl font-bold pt-16 xl:pt-16 xl:text-9xl text-center w-full">Contact</h1>
      <p class="pt-12 text-center">nossa.schaefer@gmail.com</p>
      <p class="text-xl pt-4 pb-4 font-bold tracking-wider text-center">I'm happy to work!</p>
    </div>
    <a href="/imprint" @click.prevent="scrollToSection('imprint')" class="block py-2 sm:py-0 pb-8"
      >Imprint</a
    >
  </section>
</template>

<script>
export default {
  name: 'ContactView',
  methods: {
    scrollToSection(sectionId) {
      const section = document.getElementById(sectionId)
      if (section) {
        const headerOffset = document.querySelector('header').offsetHeight
        const elementPosition = section.getBoundingClientRect().top
        const offsetPosition = elementPosition + window.scrollY - headerOffset

        window.scrollTo({
          top: offsetPosition,
          behavior: 'smooth',
        })

        history.replaceState(null, '', `/${sectionId}`)
      }
    },
  },
}
</script>
