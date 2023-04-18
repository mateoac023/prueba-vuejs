<template>
  <div>{{ text }}</div>
  <div>{{ algo }}</div>
</template>

<script>
import base from "@/mixins/base";

export default {
  name: "App",
  mixins: [base],
  data() {
    return {
      text: "Hola Vue",
    };
  },
  beforeCreate() {
    console.log("beforeCreate", this.$data, this.$el);
  },
  created() {
    console.log("created", this.$data, this.$el);
  },
  mounted() {
    console.log("mounted", this.$data, this.$el);
  },
};
</script>
