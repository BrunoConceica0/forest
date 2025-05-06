<script setup>
import ButtonReserve from "../../../components/ButtonReserve.vue";
</script>

<template>
  <section>
    <div class="m-auto flex flex-col items-center justify-center">
      <div class="relative">
        <video
          class="rounded-xl h-[30rem] max-w-[150rem] object-cover"
          width="1500"
          height="240"
          autoplay
          muted
          loop
        >
          <source src="../../../img/video_sol.mp4" type="video/mp4" />
        </video>
        <div
          class="absolute top-0 left-0 w-full h-full flex items-center justify-center"
        >
          <ButtonReserve class="absolute top-50% left-10" />
        </div>
      </div>
    </div>
  </section>
</template>

<style></style>
