<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
export default {
  name: "AppComponent",
  components: {
    HeaderComponent,
    FooterComponent,
  },
};
</script>

<template>
  <div id="app">
    <HeaderComponent />
    <router-view class="main-content" />
    <FooterComponent class="footer" />
  </div>
</template>

<style lang="scss" scoped></style>
