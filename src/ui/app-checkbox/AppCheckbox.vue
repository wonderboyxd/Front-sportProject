<template>
  <section class="app-checkbox">
    <input class="checkbox" type="checkbox" />
    <label class="label">{{ item.title }}</label>
  </section>
</template>

<script lang="ts">
import { PropType } from "vue";
import { defineComponent } from "vue";
interface IItem {
  title: string;
}
export default defineComponent({
  props: {
    item: {
      type: Object as PropType<IItem>,
    },
  },
  data() {
    return {};
  },
  methods: {},
});
</script>

<style lang="scss">
@import "style.scss";
</style>
