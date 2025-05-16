<template>
  <div class="">
    <button
      v-if="!menu"
      @click="opneMenu"
      class="capitalize text-black text-sm cursor-pointer font-sans-serif bg-gradient-to-b from-verde-300 to-verde-400 px-4 py-2 rounded-full shadow-[0_0_2px_1px_var(--color-verde-200)]"
    >
      menu
    </button>
    <div
      class="fixed inset-0 z-50 bg-black opacity-50 flex justify-center items-center"
      v-else
    >
      <nav
        class="bg-verde-200 p-6 rounded-xl shadow-lg z-60 w-3/4 max-w-md text-center"
      >
        <ul
          class="flex flex-col text-white gap-4text-xl font-sans-serif text-balance"
        >
          <li
            class="cursor-pointer p-4"
            v-for="(navigation, index) in navigations"
            :key="index"
          >
            {{ navigation.name }}
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { navigationLinks } from "@/assets/view/constant/headerNav";
const navigations = navigationLinks;
const menu = ref(false);
const opneMenu = () => {
  menu.value = true;
};

const props = defineProps(["menu"]);
</script>

<style></style>
