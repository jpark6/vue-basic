<template>
  <div>
    <app-header v-bind:propsdata="headerStr" v-on:renew="renewStr" />
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
  methods: {
    renewStr: function () {
      this.headerStr = this.headerStr === "Header" ? "Hi!!!" : "Header";
    },
  },
};
</script>

<style></style>
