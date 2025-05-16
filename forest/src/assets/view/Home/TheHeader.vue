<template>
  <header class="container mx-auto">
    <ClimateComponent class="pt-4 pb-2" />
    <article class="flex justify-between py-4 items-center">
      <div>
        <img src="../../../img/forest.svg" alt="Logo da Forest" />
      </div>
      <nav>
        <ul
          class="flex flex-row gap-4 text-white text-xl font-sans-serif text-balance max-lg:hidden"
        >
          <li
            class="cursor-pointer px-2 py-4"
            v-for="(navigation, index) in navigations"
            :key="index"
          >
            <a
              class="border-b-2 border-transparent hover:border-b-2 hover:border-white trabnsition-all duration-300 ease-in-out py-1"
              :href="navigation.link"
              >{{ navigation.name }}</a
            >
          </li>
        </ul>
        <ModalHeaderComponent class="lg:hidden" />
      </nav>
    </article>
  </header>
</template>

<script setup>
import { ref } from "vue";
import { navigationLinks } from "@/assets/view/constant/headerNav";
import ClimateComponent from "@/components/ClimateComponent.vue";
import ModalHeaderComponent from "@/components/ModalHeader.vue";

const navigations = navigationLinks;

const menu = ref(false);
const opneMenu = () => {
  menu.value = true;
  console.log(menu.value);
};
</script>

<style></style>
