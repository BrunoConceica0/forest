<script setup>
import ButtonReserve from "../../../components/ButtonReserve.vue";
</script>

<template>
  <main>
    <div class="m-auto flex flex-col items-center justify-center shadow-lg">
      <div class="relative">
        <video
          class="rounded-xl h-[40rem] max-w-[150rem] object-cover"
          width="1500"
          height="240"
          autoplay
          muted
          loop
        >
          <source src="../../../img/video_chuva.mp4" type="video/mp4" />
        </video>
        <div
          class="absolute top-0 left-0 w-full h-full flex items-center justify-center:"
        >
          <ButtonReserve class="absolute top-50% left-10" />

          <h1
            class="absolute bottom-40 text-white text-balance font-serif text-5xl ml-10"
          >
            Venha Experimentar <br />a Vida na Floresta
          </h1>

          <div class="absolute bottom-0 ml-10 *:text-white">
            <p class="text-lg">
              Melhores locais para visitar
              <a class="border-b-2 hover:border-none" href=""> 2049</a>
            </p>
            <div class="flex flex-col gap-4">
              <p class="uppercase font-semibold">recomendado por</p>
              <div class="flex gap-4">
                <img
                  class="w-32"
                  src="../../../img/parceiros/wildbeast.svg"
                  alt="Wildbeast"
                />
                <span>|</span>Revista Nacional
              </div>
            </div>
          </div>
        </div>
      </div>
      <section class="grid grid-cols-[1fr_2fr] gap-4 container my-16">
        <div class="*:text-white row-span-full">
          <h2
            class="capitalize text-5xl text-balance font-serif mb-10 col-span-full"
          >
            Refúgio Natural
          </h2>
          <ul
            class="*:mb-2 *:text-xl text-balance *:flex *:items-center *:gap-2"
          >
            <li>
              <span class="h-0.2 w-6 inline-block neon"></span>Experimente a
              natureza de perto
            </li>
            <li>
              <span class="h-0.2 w-6 inline-block neon"></span>Conecte-se com a
              natureza
            </li>
            <li class="flex items-center gap-2">
              <span class="h-0.2 w-6 inline-block neon"></span>Desconecte-se do
              digital
            </li>
            <li>
              <span class="h-0.2 w-6 inline-block neon"></span>Observe a vida
              selvagem
            </li>
            <li>
              <span class="h-0.2 w-6 inline-block neon"></span>Escolha a sua
              cabine preferida
            </li>
          </ul>
        </div>
        <div
          class="col-span-1 row-span-2 grid grid-cols-[2fr_1fr] gap-8 *:*:object-cover *:*:rounded-lg *:*:shadow-lg"
        >
          <div class="col-span-full relative">
            <img class="h-52 w-full" src="../../../img/casa1.jpg" alt="" />
            <span
              class="absolute uppercase text-sm/none top-0 right-0 text-white bg-verde-950/60 rounded-full py-2 px-4 m-2"
              >Ruby</span
            >
          </div>
          <div class="relative">
            <img src="../../../img/casa2.jpg" alt="" />
            <span
              class="absolute uppercase text-sm/none top-0 right-0 text-white bg-verde-950/60 rounded-full py-2 px-4 m-2"
              >Emerald</span
            >
          </div>
          <div class="relative">
            <img class="h-full" src="../../../img/casa3.jpg" alt="" />
            <span
              class="absolute uppercase text-sm/none top-0 right-0 text-white bg-verde-950/60 rounded-full py-2 px-4 m-2"
              >Saphire</span
            >
          </div>
        </div>
      </section>
    </div>
  </main>
</template>

<style></style>
