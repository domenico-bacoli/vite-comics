<script>
import AppNavbar from "./components/AppNavbar.vue";
import AppJumbo from "./components/AppJumbo.vue";
import AppHeader from "./components/AppHeader.vue";

export default {
  data() {
    return {

    }
  },

  components: {
    AppNavbar,
    AppJumbo,
    AppHeader,
  }
}

</script>

<template>
  <div>
    <AppNavbar></AppNavbar>
    <AppJumbo></AppJumbo>
    <AppHeader></AppHeader>
  </div>
</template>

<style scoped></style>
