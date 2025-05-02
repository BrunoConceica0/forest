<template>
  <header class="container mx-auto">
    <ClimateComponent class="pt-4 pb-2" />
    <article class="flex justify-between p-4 items-center">
      <div>
        <img src="../../../img/forest.svg" alt="Logo da Forest" />
      </div>
      <nav>
        <ul
          class="flex flex-row gap-4 text-white text-xl font-sans-serif text-balance"
        >
          <li
            class="cursor-pointer px-2 py-4"
            v-for="(navigation, index) in navigations"
            :key="index"
          >
            <a :href="navigation.link">{{ navigation.name }}</a>
          </li>
        </ul>
      </nav>
    </article>
  </header>
</template>

<script>
import { navigationLinks } from "../constant/headerNav";
import ClimateComponent from "../../../components/ClimateComponent.vue";
// import { ref } from "vue";
export default {
  name: "TheHeader",
  components: {
    ClimateComponent,
  },
  setup() {
    // const user = ref([]);
    return {
      navigations: navigationLinks,
    };
  },
};
</script>

<style></style>
