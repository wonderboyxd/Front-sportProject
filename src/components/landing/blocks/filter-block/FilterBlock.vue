<template>
  <section class="filter-block">
    <div class="filter-block__content">
      <div class="filter-block__content-header">
        <p class="filter-block__content-header-title">{{ category }}</p>
        <app-button class="filter-block__content-header-button" />
      </div>
      <app-checkbox
        v-for="(item, index) of categoryTitleList"
        :item="item"
        :key="index"
      />
    </div>
    <div class="filter-block__content">
      <div class="filter-block__content-header">
        <p class="filter-block__content-header-title">{{ regions }}</p>
        <app-button class="filter-block__content-header-button" />
      </div>
      <app-checkbox
        v-for="(item, index) of regionsTitleList"
        :item="item"
        :key="index"
      />
    </div>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AppButton from "@/ui/app-button/AppButton.vue";
import AppCheckbox from "@/ui/app-checkbox/AppCheckbox.vue";
export default defineComponent({
  components: {
    AppButton,
    AppCheckbox,
  },
  data() {
    return {
      category: "Категории",
      regions: "Регионы",
      categoryTitleList: [
        {
          title: "Футбол",
        },
        {
          title: "Волейбол",
        },
        {
          title: "Волейбол",
        },
        {
          title: "Волейбол",
        },
        {
          title: "Волейбол",
        },
        {
          title: "Футбол",
        },
      ],
      regionsTitleList: [
        {
          title: "Томская область",
        },
        {
          title: "Республика Татарстан",
        },
        {
          title: "Омская область",
        },
        {
          title: "Республика Коми",
        },
        {
          title: "Красноярский край",
        },
      ],
    };
  },
});
</script>

<style lang="scss">
@import "style.scss";
</style>
