<template>
  <section>
    <section class="infos-page">
      <h1 class="subtitle">Programme</h1>
      <Separator/>
      <img width="64" src="~/assets/images/icons8-horloge-96.png">

      <div class="timeline">
        <div>
          <h2>15h00 - Mairie de Saint Priest</h2>
          <p>Passage des futurs mariés devant le maire.</p>
        </div>
        <div>
          <h2>16h00 - Pause photos</h2>
          <p>Souriez, vous êtes filmés !</p>
        </div>
        <div>
          <h2>17h30 - Départ pour le Domaine du Ruisseau</h2>
          <p>Suivez-nous à la ZAC de la Tuillère, 69510 Thurins</p>
        </div>
        <div>
          <h2>18h15 - Cocktail Apéritif</h2>
          <p>Trinquons ensemble</p>
        </div>
        <div>
          <h2>20h30 - Diner barbecue</h2>
          <p>Bon appetit</p>
        </div>
        <div>
          <h2>23h30 - Alors on danse ?</h2>
          <p>Tous sur la piste jusqu'au petit matin</p>
        </div>
      </div>
    </section>
  </section>
</template>
<script>
import Separator from "~/components/Separator.vue";
export default {
  components: {
    Separator
  }
};
</script>


<style lang="scss">
.timeline {
  h2 {
    color: #ff5757;
    font-family: "Niconne";
    font-size: 1.5em;
  }
  p {
    margin-top: 15px;
    margin-bottom: 20px;
    font-family: "Lobster";
  }
}
</style>
