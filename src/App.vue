<script>
import AppNavbar from "./components/AppNavbar.vue";
import AppMain from "./components/AppMain.vue";
import AppBluBandSection from "./components/AppBluBandSection.vue";
import AppFooterBottom from "./components/AppFooterBottom.vue";
import AppFooterTop from "./components/AppFooterTop.vue";

export default {
  data() {
    return {

    }
  },

  components: {
    AppNavbar,
    AppMain,
    AppBluBandSection,
    AppFooterBottom,
    AppFooterTop,
  }
}

</script>

<template>
  <div>
    <AppNavbar></AppNavbar>
    <AppMain></AppMain>
    <AppFooterTop></AppFooterTop>
    <AppFooterBottom></AppFooterBottom>
  </div>
</template>

<style scoped></style>
