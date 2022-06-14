<template>
  <main class="app">
    <div class="app_wrapper">
      <WeatherForm></WeatherForm>
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import WeatherForm from "@/components/WeatherForm.vue";

export default defineComponent({
  name: "HomeView",
  components: { WeatherForm },
});
</script>
