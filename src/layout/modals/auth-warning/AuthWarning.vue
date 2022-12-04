<template>
  <div class="auth-warning">
    <div class="auth-warning__icon">
      <img src="@/assets/auth-warning-img/icon-warning.svg" alt="Warning" />
    </div>
    <div class="auth-warning__text">
      <p>Чтобы создать мероприятие, авторизируйтесь или зарегистрируйтесь</p>
    </div>
    <div class="auth-warning__button" @click="true">
      <img src="@/assets/auth-warning-img/icon-warning-close.svg" alt="Close" />
    </div>
  </div>
</template>

<script lang="ts">
export default {
  components: {},
};
</script>

<style lang="scss">
@import "./style";
</style>
