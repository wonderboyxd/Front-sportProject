<template>
  <section class="events-block">
    <div class="events-block__header">
      <h2 class="events-block__header-title">Список мероприятий</h2>
      <app-button :title="'Создать мероприятие'" />
    </div>
    <div class="events-block__filter">
      <h2 class="events-block__filter-title">Фильтры</h2>
      <filter-block />
    </div>
    <div class="events-block__content"></div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AppButton from "@/ui/app-button/AppButton.vue";
import FilterBlock from "@/components/landing/blocks/filter-block/FilterBlock.vue";
export default defineComponent({
  components: {
    AppButton,
    FilterBlock,
  },
  data() {
    return {};
  },
});
</script>

<style lang="scss">
@import "style.scss";
</style>
