<template>
  <div
    class="flex gap-1 items-center *:bg-verde-900 *:text-verde-300 *:text-base *:rounded-lg *:py-2 *:px-4 *:font-sans-serif"
  >
    <div class="">
      <span
        class="size-2 inline-block relative bg-verde-400 rounded-full -left-5 border-1 shadow-[0_0_6px_1px_var(--color-verde-200)]"
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
