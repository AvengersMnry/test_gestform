<template>
  <div class="rules">
    <h1>Test technique | Consignes</h1>
    <ul>
      <li>
        Créer un programme informatique oeuvrant sur une liste de nombre entier
        entre -1000 et 1000.
      </li>
      <li>Si le nombre est divisible par 3 : afficher GESTE</li>
      <li>Si le nombre est divisible par 5 : afficher FORME</li>
      <li>Si le nombre est divisible par 3 ET 5 : afficher GESTFORM</li>
      <li>Sinon, afficher la valeur du nombre.</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Consignes",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
li {
  list-style: square;
  text-align: center;
  margin-bottom: 2em;
}
.rules {
  background-color: rgb(255, 102, 0, 0.3);
  width: 50%;
}
@media (max-width: 1024px) {
  .rules {
    width: 100%;
    margin-top: 2%;
    padding-bottom: 1%;
  }
}
</style>
