<template>
  <button @click="show = !show">Menú</button>
  <transition name="fade">
    <MenuPrueba v-if="show" />
  </transition>
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

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade.leave-to {
  opacity: 0;
}
</style>
