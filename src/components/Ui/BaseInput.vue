<template>
  <input :value="modelValue" type="text" @input="updateValue" />
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "BaseInput",
  props: {
    modelValue: {
      type: String,
      required: true,
      default: "",
    },
  },
  methods: {
    updateValue(event: any) {
      this.$emit("update:modelValue", event.target.value);
    },
  },
});
</script>

<style scoped></style>
