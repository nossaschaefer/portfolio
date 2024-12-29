<template>
  <section
    id="projects"
    class="min-h-screen flex flex-col items-center justify-center w-full xl:px-20 md:pt-20"
  >
    <h1 class="font text-8xl tracking-tight sm:text-9xl text-center font-bold pt-16 mb-8">
      Projects
    </h1>
    <div class="flex flex-col gap-[6rem] p-4 md:p-6 2xl:pt-16 items-center w-full max-w-[1490px]">
      <!-- TooGoodToThrow App Card -->
      <div
        class="flex flex-col lg:flex-row gap-8 relative group hover:-translate-y-2 transition-transform duration-300 ease-in-out w-full"
      >
        <!-- Card Content -->
        <div class="flex-1 lg:flex-col lg:justify-between lg:pr-6">
          <h3 class="text-[2.7rem] font-bold text-indigo-800">TooGoodToThrow Web App</h3>
          <p class="pt-4 pb-4">
            If you see something on the street that is too good to throw away, you can take a
            picture, upload it to the app and share it with others. You can also see what others
            have posted and filter by category.
          </p>
          <div class="text-indigo-600 mt-2 leading-relaxed flex gap-2 pt-2">
            <p class="border-2 border-black p-1">Flask</p>
            <p class="border-2 border-black p-1">Python</p>
            <p class="border-2 border-black p-1">Bootstrap</p>
          </div>
          <div class="mt-4 justify-start flex gap-2">
            <a
              href="https://flask-app-toogoodtothrow.fly.dev/"
              target="_blank"
              class="inline-block px-4 py-2 bg-purple-500 text-white rounded-3xl font-medium hover:bg-purple-600 transition-colors"
            >
              Live Site
            </a>

            <a
              href="https://github.com/nossaschaefer/flask-app-toogoodtothrow"
              target="_blank"
              class="inline-block px-4 py-2 bg-gray-800 text-white rounded-3xl font-medium hover:bg-gray-900 transition-colors"
            >
              GitHub
            </a>
          </div>
        </div>

        <!-- Image -->
        <div class="flex-1">
          <div class="h-full aspect-[14.5/8]">
            <img
              src="@/assets/Bildschirmfoto2024-TooGoodToThrow.png"
              alt="TooGoodToThrow Web App"
              class="h-full object-cover rounded group-hover:scale-105 transition-transform duration-300"
            />
          </div>
        </div>
      </div>

      <!-- Learnified App Card -->
      <div
        class="flex flex-col lg:flex-row gap-8 relative group hover:-translate-y-2 transition-transform duration-300 ease-in-out w-full"
      >
        <!-- Card Content -->
        <div class="flex-1 lg:pr-6">
          <h3 class="text-5xl font-bold text-indigo-800">Learnified Web App</h3>
          <p class="pt-4 pb-4">
            With this app, you can test and expand your knowledge in HTML & CSS, JavaScript, and
            Vue.js. In the quiz, you can score points and compete with other users on the
            leaderboard. You can even add your own cards, continually growing your knowledge.
          </p>
          <div class="text-indigo-600 mt-2 leading-relaxed flex gap-2 pt-2">
            <p class="border-2 border-black p-1">Vue.js</p>
            <p class="border-2 border-black p-1">JavaScript</p>
          </div>
          <div class="mt-4 justify-start flex gap-2">
            <a
              href="https://learnified.netlify.app/"
              target="_blank"
              class="inline-block px-4 py-2 bg-purple-500 text-white rounded-3xl font-medium hover:bg-purple-600 transition-colors"
            >
              Live Site
            </a>

            <a
              href="https://github.com/nossaschaefer/flask-app-toogoodtothrow"
              target="_blank"
              class="inline-block px-4 py-2 bg-gray-800 text-white rounded-3xl font-medium hover:bg-gray-900 transition-colors"
            >
              GitHub
            </a>
          </div>
        </div>

        <!-- Image -->
        <div class="flex-1">
          <div class="h-full aspect-[14.5/8]">
            <img
              src="@/assets/Bildschirmfoto-Learnified-App.png"
              alt="TooGoodToThrow Web App"
              class="h-full object-cover rounded group-hover:scale-105 transition-transform duration-300"
            />
          </div>
        </div>
      </div>

      <!-- Todo App Card -->
      <div
        class="flex flex-col lg:flex-row gap-8 relative group hover:-translate-y-2 transition-transform duration-300 ease-in-out w-full"
      >
        <!-- Card Content -->
        <div class="flex-1 lg:flex-col lg:justify-between lg:pr-6">
          <h3 class="text-5xl font-bold text-indigo-800">Todo Web App</h3>
          <p class="pt-4 pb-4">
            With this app, you can create a list of tasks, mark them as done, and delete them. And
            you can also filter them by status.
          </p>
          <div class="text-indigo-600 mt-2 leading-relaxed flex gap-2 pt-2">
            <p class="border-2 border-black p-1">Flask</p>
            <p class="border-2 border-black p-1">Python</p>
            <p class="border-2 border-black p-1">Bootstrap</p>
          </div>
          <div class="mt-4 justify-start flex gap-2">
            <a
              href="https://todo-app-vue-vite.netlify.app/"
              target="_blank"
              class="inline-block px-4 py-2 bg-purple-500 text-white rounded-3xl font-medium hover:bg-purple-600 transition-colors"
            >
              Live Site
            </a>

            <a
              href="https://github.com/nossaschaefer/flask-app-toogoodtothrow"
              target="_blank"
              class="inline-block px-4 py-2 bg-gray-800 text-white rounded-3xl font-medium hover:bg-gray-900 transition-colors"
            >
              GitHub
            </a>
          </div>
        </div>

        <!-- Image -->
        <div class="flex-1">
          <div class="h-full aspect-[14.5/8]">
            <img
              src="@/assets/Bildschirmfoto-Todo-App.png"
              alt="TooGoodToThrow Web App"
              class="h-full object-cover rounded group-hover:scale-105 transition-transform duration-300"
            />
          </div>
        </div>
      </div>

      <!-- Color Mixer App Card -->
      <div
        class="flex flex-col lg:flex-row gap-8 relative group hover:-translate-y-2 transition-transform duration-300 ease-in-out w-full"
      >
        <!-- Card Content -->
        <div class="flex-1 lg:flex-col lg:justify-between lg:pr-6">
          <h3 class="text-5xl font-bold text-indigo-800">Color Mixer Web App</h3>
          <p class="pt-4 pb-4">
            This app lets you mix colors and see the result. It also gives out the rgb color code.
          </p>
          <div class="text-indigo-600 mt-2 leading-relaxed flex gap-2 pt-2">
            <p class="border-2 border-black p-1">Flask</p>
            <p class="border-2 border-black p-1">Python</p>
            <p class="border-2 border-black p-1">Bootstrap</p>
          </div>
          <div class="mt-4 justify-start flex gap-2">
            <a
              href="https://color-mixer-app-vue.netlify.app"
              target="_blank"
              class="inline-block px-4 py-2 bg-purple-500 text-white rounded-3xl font-medium hover:bg-purple-600 transition-colors"
            >
              Live Site
            </a>

            <a
              href="https://github.com/nossaschaefer/flask-app-toogoodtothrow"
              target="_blank"
              class="inline-block px-4 py-2 bg-gray-800 text-white rounded-3xl font-medium hover:bg-gray-900 transition-colors"
            >
              GitHub
            </a>
          </div>
        </div>

        <!-- Image -->
        <div class="flex-1">
          <div class="h-full aspect-[14.5/8]">
            <img
              src="@/assets/Color-Mixer.png"
              alt="TooGoodToThrow Web App"
              class="h-full object-cover rounded group-hover:scale-105 transition-transform duration-300"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProjectsView',
}
</script>

<style>
.font {
  font-family: 'Outfit', serif;
}
.aspect-ratio-1.7 {
  position: relative;
  width: 100%;
  padding-bottom: 58.82%; /* 1 / 1.7 * 100% */
}
.aspect-ratio-1.7 img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
