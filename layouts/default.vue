<template>
  <section class="main">
    <Menu class="floatleft"/>
    <div class="floatleft container">
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

.main {
  display: flex;
  justify-content: space-around;
  align-items: center;
  max-width: 1000px;
  margin: 0 auto;
}

@media screen and (max-width: 1000px) {
  .main {
    display: block;
  }
  .floatleft {
    float: left;
    width: 100%;
  }
}
</style>
