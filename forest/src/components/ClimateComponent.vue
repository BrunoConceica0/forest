<template>
  <div
    class="flex gap-1 items-center relative *:bg-verde-900 *:text-verde-300 *:text-base *:rounded-lg *:py-2 *:px-4 *:font-sans-serif"
  >
    <div class="">
      <span
        class="neon inline-block border w-2 h-2 bg-verde-200 absolute top-1/2 -left-1"
      ></span
      >{{ info.dayOffWeek }}
    </div>
    <div class="">26º</div>

    <div class="">🌤️</div>
  </div>
</template>
<script>
import { reactive, onMounted } from "vue";
export default {
  name: "ClimateComponent",

  setup() {
    const info = reactive({
      dayOffWeek: "",
      temperature: null,
    });

    const climate = () => {
      const data = new Date();
      const day = [
        "Domingo",
        "Segunda",
        "Terça",
        "Quarta",
        "Quinta",
        "Sexta",
        "Sábado",
      ];

      info.dayOffWeek = day[data.getDay()];
    };
    onMounted(() => {
      climate();
    });
    return {
      info,
    };
  },
};
</script>
<style></style>
