<template>
  <section>
    <section class="infos-page">
      <h1 class="subtitle">Programme</h1>
      <img class="icon" src="~/assets/images/icons8-horloge-96.png">

      <div class="timeline">
        <div v-for="step in steps" :key="step.id">
          <h2>{{step.hour}} - {{step.title}}</h2>
          <p>{{step.desc}}</p>
        </div>
      </div>
    </section>
  </section>
</template>
<script>
import Separator from "~/components/Separator.vue";
export default {
  data() {
    return {
      steps: [
        {
          id: 0,
          hour: "15h00",
          title: "Mairie de Saint Priest",
          desc: "Passage des futurs mariés devant le maire."
        },
        {
          id: 1,
          hour: "16h00",
          title: "Pause photos",
          desc: "Souriez, vous êtes filmés !"
        },
        {
          id: 2,
          hour: "17h30",
          title: "Direction le Domaine du Ruisseau",
          desc: "Suivez-nous à la ZAC de la Tuillère, 69510 Thurins."
        },
        {
          id: 3,
          hour: "18h15",
          title: "Cocktail Apéritif",
          desc: "Trinquons ensemble."
        },
        {
          id: 4,
          hour: "20h30",
          title: "Diner barbecue et gateau",
          desc: "Bon appetit !"
        },
        {
          id: 4,
          hour: "23h30",
          title: "23h30 - Alors on danse ?",
          desc: "Tous sur la piste jusqu'au petit matin..."
        }
      ]
    };
  },
  components: {
    Separator
  }
};
</script>


<style lang="scss">
.timeline {
  h2 {
    color: #ff5757c7;
    font-family: "Niconne";
    font-size: 1.45em;
  }
  p {
    margin-top: 15px;
    margin-bottom: 20px;
    font-family: "Lobster";
  }
}
</style>
