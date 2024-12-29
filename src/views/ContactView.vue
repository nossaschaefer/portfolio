<template>
  <section
    id="contact"
    class="min-h-screen flex flex-col items-center justify-between w-full md:pt-20"
  >
    <div class="flex-col justify-center">
      <h1 class="font text-8xl font-bold pt-16 xl:pt-16 xl:text-9xl text-center w-full">Contact</h1>
      <p class="pt-12 text-center text-2xl">nossa.schaefer@gmail.com</p>
      <p class="text-3xl pt-4 pb-4 font-bold tracking-wider text-center">I'm happy to work!</p>
      <div class="flex justify-center gap-4 pt-4">
        <!-- GitHub -->
        <a
          href="https://github.com/username"
          target="_blank"
          rel="noopener noreferrer"
          class="text-gray-700 hover:text-gray-900 transition-colors duration-200"
        >
          <i class="fab fa-github text-4xl"></i>
        </a>
        <!-- LinkedIn -->
        <a
          href="https://linkedin.com/in/username"
          target="_blank"
          rel="noopener noreferrer"
          class="text-[#0a66c2] hover:text-[#085ca0] transition-colors duration-200"
        >
          <i class="fab fa-linkedin text-4xl"></i>
        </a>
      </div>
    </div>

    <div class="flex items-center">
      <button
        @click="toggleText"
        :class="{
          'text-xl': !isTextVisible,
          'pb-6': !isTextVisible,
          'text-8xl font-bold transition-all': isTextVisible,
          'pt-40': isTextVisible,
        }"
        class="font"
      >
        ➤ Imprint
      </button>
    </div>

    <section
      v-if="isTextVisible"
      id="imprint"
      class="min-h-screen flex flex-col items-center w-full xl:px-20"
    >
      <div class="flex flex-col px-6 items-center justify-center w-full max-w-[1490px]">
        <h2 class="text-xl pt-8 font-medium">Information according to § 5 TMG</h2>
        <p class="text-center">
          Nossa Schäfer<br />
          Erlanger Str., Berlin <br />nossa.schaefer@gmail.com
        </p>
        <br />
        <h2 class="text-xl font-medium">Liability for links on this website</h2>
        <p class="text-pretty pt-2">
          My website contains links to other websites, for whose content I am not responsible. There
          is no liability for linked websites, because I had and have no knowledge of illegal
          activities, I have not noticed any such illegal activities and I will remove links
          immediately if I become aware of any illegal activities. If you notice illegal links on my
          website, please contact me. You will find the contact details above.
        </p>
        <br />
        <h2 class="text-xl font-medium">Copyright information</h2>
        <p class="text-pretty pt-2">
          The contents and works on these pages created by me are subject to German copyright law.
          The duplication, processing, distribution and any kind of utilization outside the limits
          of copyright law require my written consent. Downloads and copies of these pages are only
          permitted for private, non-commercial use. If necessary, I will legally pursue the
          unauthorized use of parts of the contents of my site. If you find content on this website
          that violates copyright law, please contact me.
        </p>
        <br />
        <h2 class="text-xl font-medium">Privacy policy</h2>
        <p class="text-pretty pt-2 pb-8">
          The use of my website is possible without giving personal data. I would like to point out
          that data transmission over the Internet (e.g. communication by e-mail) can have security
          gaps. A complete protection of data against access by third parties is not possible. The
          use of contact data published within the framework of the imprint obligation by third
          parties for sending advertising and information material not explicitly requested is
          hereby expressly prohibited. I expressly reserve the right to take legal action in the
          event of unsolicited sending of advertising information by, for example, spam e-mails.
        </p>
      </div>
    </section>
  </section>
</template>

<script>
export default {
  data() {
    return {
      isTextVisible: false, // Versteckter Text initial nicht sichtbar
    }
  },
  methods: {
    toggleText() {
      this.isTextVisible = !this.isTextVisible // Zustand umschalten
    },
  },
}
</script>

<style>
/* Optional: Importiere Font Awesome CSS */
@import '@fortawesome/fontawesome-free/css/all.min.css';
</style>
