<template>
  <Header />
  <Home />
</template>

<script lang="ts">
import Home from "./pages/Home.vue";
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: { Header, Home },
};
</script>

<style></style>
