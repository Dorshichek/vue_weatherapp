<template>
  <form class="weather-app">
    <BaseInput
      v-model="city"
      class="weather-app__input"
      placeholder="Введите город"
      type="text"
    />
    <button class="weather-app__search" type="submit"></button>
  </form>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import BaseInput from "@/components/Ui/BaseInput.vue";

export default defineComponent({
  name: "WeatherForm",
  components: { BaseInput },
  data() {
    return {
      city: "",
    };
  },
  props: {},
});
</script>

<style lang="scss" scoped></style>
