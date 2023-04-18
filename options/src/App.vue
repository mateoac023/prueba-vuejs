<template>
  <HomeSetup first-name="Mateo" last-name="Arias"></HomeSetup>
</template>

<script>
import HomeSetup from "./components/HomeSetup.vue";
import { provide } from "vue";

export default {
  name: "App",
  components: {
    HomeSetup,
  },
  setup() {
    provide("username", "MateoNerd");
  },
};
</script>
