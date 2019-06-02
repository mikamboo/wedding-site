<template>
  <section class="header">
    <NLink to="/">
      <h1 class="title">Sidonie & Michaël</h1>
    </NLink>
    <Separator/>
    <h2 class="subtitle">Se diront Oui ...
      <br>Le Samedi 31 Août 2019
    </h2>
    <div class="links">
      <a
        to="/rsvp"
        class="button--green typeform-share"
        href="https://michael-po.typeform.com/to/gPDMft"
        data-mode="drawer_left"
        data-auto-open="false"
        data-hide-headers="false"
        data-hide-footer="false"
        target="_blank"
      >Confirmer présence</a>
      <MenuTabs></MenuTabs>
    </div>
  </section>
</template>
<script>
import Separator from "~/components/Separator.vue";
import MenuTabs from "~/components/MenuTabs.vue";

export default {
  components: {
    Separator,
    MenuTabs
  },
  mounted() {
    //Load Typeform
    (function() {
      var qs,
        js,
        q,
        s,
        d = document,
        gi = d.getElementById,
        ce = d.createElement,
        gt = d.getElementsByTagName,
        id = "typef_orm_share",
        b = "https://embed.typeform.com/";
      if (!gi.call(d, id)) {
        js = ce.call(d, "script");
        js.id = id;
        js.src = b + "embed.js";
        q = gt.call(d, "script")[0];
        q.parentNode.insertBefore(js, q);
      }
    })();
  }
};
</script>
<style lang="scss">
.header {
  text-align: center;
  a {
    text-decoration: none;
    &:visited {
      color: #2E495E;
    }
    &:hover {
      color: #FFF;
    }
  }
}

.title {
  font-family: "Niconne";
  display: block;
  font-weight: 400;
  color: #e4a9a0;
  font-size: 3.8em;
}

.subtitle {
  font-weight: 300;
  font-size: 2em;
  color: #ab7329;
  padding-bottom: 5px;
  font-family: "Niconne";
}

.links {
  padding: 10px;
}
</style>

