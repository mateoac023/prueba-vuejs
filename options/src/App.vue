<template>
  <button @click="show = !show">Menú</button>
  <MenuPrueba v-if="show" />
</template>

<script>
import MenuPrueba from "./components/MenuPrueba.vue";
export default {
  name: "App",
  components: { MenuPrueba },
  data() {
    return {
      show: false,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
