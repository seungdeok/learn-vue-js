<template>
  <header>
    <h1>Header {{ data }}</h1>
    <button v-on:click="sendEvent">Send</button>
  </header>
</template>

<script>
export default {
  props: ["data"],
  methods: {
    sendEvent: function () {
      this.$emit("update");
    },
  },
};
</script>

<style></style>
