<template>
  <section>
    <div>
      <!-- <Logo :width="300"/> -->
      <h1 class="title">Faire-Part</h1>
      <!-- <h2 class="subtitle">31.08.2019</h2> -->
      <img class="flyer" src="~/assets/images/sido-mike-1.png" alt="Sido & Mike">
      <div class="links">
        <NLink to="/rsvp" class="button--green">Confimer présende</NLink>
        <NLink to="/infos" class="button--grey">Informations utiles</NLink>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from "~/components/Logo.vue";
import IconLink from "~/components/IconLink.vue";

export default {
  components: {
    Logo,
    IconLink
  }
};
</script>

<style scoped>
.flyer {
  width: 80%;
}
.title {
  font-family: "Niconne";
  display: block;
  font-weight: 400;
  color: #2E495E;
  letter-spacing: 1px;
  font-size: 4.5em;
}

.subtitle {
  font-weight: 300;
  font-size: 3em;
  color: #2E495E;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
