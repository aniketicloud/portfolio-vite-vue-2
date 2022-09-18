<script>
import HeaderComponent from "./components/HeaderComponent.vue";
export default {
  name: "AppComponent",
  components: {
    HeaderComponent,
  },
};
</script>

<template>
  <div id="app">
    <HeaderComponent />
    <router-view />
  </div>
</template>

<style lang="scss" scoped></style>
