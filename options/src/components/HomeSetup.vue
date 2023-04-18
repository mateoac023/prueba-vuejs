<template>
  <div>FullName: {{ fullname }}</div>
</template>

<script>
import { computed, ref } from "vue";

export default {
  setup() {
    const firstname = ref("Mateo");
    const lastname = ref("Arias");

    const fullname = computed(() => {
      return `${firstname.value} ${lastname.value}`;
    });

    return {
      fullname,
    };
  },
};
</script>
