<template>
  <div>
    <ModalPrueba />
  </div>
</template>

<script>
import ModalPrueba from "./components/ModalPrueba.vue";
export default {
  name: "App",
  components: {
    ModalPrueba,
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
