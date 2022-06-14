<template>
  <HomeView></HomeView>
</template>

<script lang="ts">
import HomeView from "@/views/HomeView.vue";
import { defineComponent } from "vue";

import "./assets/styles/style.scss";

export default defineComponent({
  name: "App",
  components: {
    HomeView,
  },
});
</script>

<style lang="scss"></style>
