<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div>
    <div class="relative bg-indigo-800">
      <div class="absolute inset-0">
        <img
          class="w-full h-full object-cover"
          src="https://www.upc.edu.pe/nosotros/campus/img/campus-san-miguel.jpg"
          alt=""
        />
        <div
          class="absolute inset-0 bg-indigo-800 mix-blend-multiply"
          aria-hidden="true"
        />
      </div>
      <div
        class="relative max-w-7xl mx-auto py-24 px-4 sm:py-32 sm:px-6 lg:px-8"
      >
        <h1
          class="
            text-4xl
            font-extrabold
            tracking-tight
            text-white
            sm:text-5xl
            lg:text-6xl
          "
        >
          En Desarrollo
        </h1>
      </div>
    </div>
    <section class="text-gray-600 body-font relative w-full">
      <div class="absolute inset-0 bg-gray-300">
        <iframe
          width="100%"
          height="100%"
          frameborder="0"
          marginheight="0"
          marginwidth="0"
          title="map"
          scrolling="no"
          src="https://maps.google.com/maps?width=100%&height=600&hl=en&q=%C4%B0zmir+(My%20Business%20Name)&ie=UTF8&t=&z=14&iwloc=B&output=embed"
          style=""
        ></iframe>
      </div>
      <div class="container px-5 py-24 mx-auto flex">
        <div
          class="
            lg:w-1/3
            md:w-1/2
            bg-white
            rounded-lg
            p-8
            flex flex-col
            md:ml-auto
            w-full
            mt-10
            md:mt-0
            relative
            z-10
            shadow-md
          "
        >
          <h2 class="text-gray-900 text-lg mb-1 font-medium title-font">
            Colocar Datos
          </h2>
          <p class="leading-relaxed mb-5 text-gray-600">
            Post-ironic portland shabby chic echo park, banjo fashion axe
          </p>
          <div class="relative mb-4">
            <label for="email" class="leading-7 text-sm text-gray-600"
              >Punto de Inicio</label
            >
            <input
              type="email"
              id="email"
              name="email"
              class="
                w-full
                bg-white
                rounded
                border border-gray-300
                focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200
                text-base
                outline-none
                text-gray-700
                py-1
                px-3
                leading-8
                transition-colors
                duration-200
                ease-in-out
              "
            />
          </div>
          <div class="relative mb-4">
            <label for="email" class="leading-7 text-sm text-gray-600"
              >Punto De Destino</label
            >
            <input
              type="email"
              id="email"
              name="email"
              class="
                w-full
                bg-white
                rounded
                border border-gray-300
                focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200
                text-base
                outline-none
                text-gray-700
                py-1
                px-3
                leading-8
                transition-colors
                duration-200
                ease-in-out
              "
            />
          </div>
          <button
            class="
              text-white
              bg-indigo-500
              border-0
              py-2
              px-6
              focus:outline-none
              hover:bg-indigo-600
              rounded
              text-lg
            "
          >
            Confirmar
          </button>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data: () => ({}),
}
</script>
