<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div class="bg-gray-900">
    <header class="bg-white">
      <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8" aria-label="Top">
        <div
          class="
            w-full
            py-6
            flex
            items-center
            justify-between
            border-b border-indigo-500
            lg:border-none
          "
        >
          <div class="flex items-center">
            <a href="#">
              <span class="sr-only">Workflow</span>
              <img
                class="h-20 w-auto"
                src="https://estudiaperu.pe/wp-content/uploads/2021/04/UPC-carreras-para-gente-que-trabaja.png"
                alt=""
              />
            </a>
            <div class="hidden ml-10 space-x-8 lg:block">
              <a
                v-for="link in navigation"
                :key="link.name"
                :href="link.href"
                class="text-base font-medium text-white hover:text-indigo-50"
              >
                {{ link.name }}
              </a>
            </div>
          </div>
          <div class="ml-10 space-x-4">
            <NuxtLink to="/home">
              <a
                href="#"
                class="
                  inline-block
                  bg-gray-800
                  py-2
                  px-4
                  border border-transparent
                  rounded-md
                  text-base
                  font-medium
                  text-white
                  hover:bg-gray-900
                "
                >Ingresar</a
              >
            </NuxtLink>
          </div>
        </div>
        <div class="py-4 flex flex-wrap justify-center space-x-6 lg:hidden">
          <a
            v-for="link in navigation"
            :key="link.name"
            :href="link.href"
            class="text-base font-medium text-white hover:text-indigo-50"
          >
            {{ link.name }}
          </a>
        </div>
      </nav>
    </header>
    <div class="mx-auto py-12 px-4 max-w-7xl sm:px-6 lg:px-8 lg:py-24">
      <div class="space-y-12">
        <div
          class="space-y-5 sm:space-y-4 md:max-w-xl lg:max-w-3xl xl:max-w-none"
        >
          <h2
            class="
              text-3xl
              font-extrabold
              text-white
              tracking-tight
              sm:text-4xl
            "
          >
            Conoce nuestro equipo
          </h2>
          <p class="text-xl text-gray-300">
            Nuestro equipo está conformado por:
          </p>
        </div>
        <ul
          role="list"
          class="
            space-y-4
            sm:grid sm:grid-cols-2 sm:gap-6 sm:space-y-0
            lg:grid-cols-3 lg:gap-8
          "
        >
          <li
            v-for="person in people"
            :key="person.name"
            class="
              py-10
              px-6
              bg-gray-800
              text-center
              rounded-lg
              xl:px-10 xl:text-left
            "
          >
            <div class="space-y-6 xl:space-y-10">
              <div class="space-y-2 xl:flex xl:items-center xl:justify-between">
                <div class="font-medium text-lg leading-6 space-y-1">
                  <h3 class="text-white">{{ person.name }}</h3>
                  <p class="text-indigo-400">{{ person.role }}</p>
                </div>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    people: [
      {
        name: 'Edinson Ricardo Cabrera Ñique (U20181E128)',
        role: 'Ingeniero De Software',
      },
      {
        name: 'Joaquin Echegoaga Ramos (U201715418)',
        role: 'Ingeniero De Software',
      },
      {
        name: 'Richard Hanns Cucho Landeo (U20181C448)',
        role: 'Ingeniero De Software',
      },
      {
        name: 'Angie Nicolle Tomasto Cahuana (U201817853)',
        role: 'Ingeniero De Software',
      },
    ],
    navigation: [],
  }),
}
</script>
