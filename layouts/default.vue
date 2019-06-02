<template>
  <section class="main">
    <Menu class="menu"/>
    <div class="content">
      <Nuxt/>
    </div>
  </section>
</template>
<script>
import Menu from "~/components/Menu.vue";
export default {
  components: {
    Menu
  }
};
</script>

<style lang="scss">
@import "../assets/sass/main.scss";
@import "../assets/sass/default-layout.scss";
</style>
