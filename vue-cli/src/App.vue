<template>
  <div>
    <app-header v-bind:propsdata="headerStr" />
    {{ str }}
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  data: () => ({
    headerStr: "Header",
    str: "Hello Vue",
  }),
  components: {
    AppHeader,
  },
};
</script>

<style></style>
