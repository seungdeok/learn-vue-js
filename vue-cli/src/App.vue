<template>
  <div>
    <app-header v-bind:data="text" v-on:update="updateEvent"></app-header>
    {{ text }}
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  data: function () {
    return {
      text: "hello world",
    };
  },
  components: {
    "app-header": AppHeader,
  },
  methods: {
    updateEvent: function () {
      this.text = "update hello world";
    },
  },
};
</script>

<style></style>
