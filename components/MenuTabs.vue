<template>
  <section>
    <div class="tabs">
      <ul>
        <li v-for="route in routes" :key="route.path">
          <NLink :to="route.path">{{route.label}}</NLink>
        </li>
      </ul>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      routes: [
        { path: "/infos/program", label: "Programme" },
        { path: "/infos/cagnotte", label: "Cagnotte" },
        { path: "/infos/contacts", label: "Contacts" }
      ]
    };
  }
};
</script>


