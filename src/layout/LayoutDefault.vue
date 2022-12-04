<template>
  <main-header />
  <auth-warning v-if="false" />
  <main>
    <router-view />
  </main>
  <events-block />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import AuthWarning from "@/layout/modals/auth-warning/AuthWarning.vue";
import MainHeader from "@/layout/main-header/MainHeader.vue";
import EventsBlock from "@/components/landing/blocks/events/EventsBlock.vue";
export default defineComponent({
  components: {
    AuthWarning,
    MainHeader,
    EventsBlock,
  },
});
</script>

<style></style>
