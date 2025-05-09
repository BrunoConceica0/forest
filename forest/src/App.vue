<template>
  <div
    class="bg-[radial-gradient(circle,_var(--color-verde-700),_var(--color-verde-900))] pb-96"
  >
    <TheHeader />
    <theMain />
  </div>
</template>

<script>
import TheHeader from "./assets/view/Home/TheHeader.vue";
import TheMain from "./assets/view/Home/TheMain.vue";
export default {
  components: { TheHeader, TheMain },
};
</script>

<style></style>
