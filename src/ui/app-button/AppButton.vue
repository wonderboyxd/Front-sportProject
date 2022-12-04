<template>
  <button class="button">
    <p class="button__title">{{ title }}</p>
  </button>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  props: {
    title: {
      type: String,
    },
  },
});
</script>

<style lang="scss">
@import "style.scss";
</style>
