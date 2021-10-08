<template>
  <div class="rules">
    <h1>Saisir un nombre entre -1000 et 1000 :</h1>
    <input type="number" id="number" max="1000" />
    <input @click="testNumber" type="button" value="Tester" id="submitNumber" />
  </div>
</template>

<script>
export default {
  name: "Consignes",
  props: {
    msg: String,
  },
  methods: {
    testNumber() {
      const myNumber = document.getElementById("number").value;

      if (myNumber % 3 === 0 && myNumber % 5 === 0) {
        alert("GESTFORM");
      } else if (myNumber % 3 === 0) {
        alert("GESTE");
      } else if (myNumber % 5 === 0) {
        alert("FORME");
      } else {
        alert(myNumber);
      }
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
li {
  list-style: square;
  text-align: right;
  margin-bottom: 2em;
}
.rules {
  background-color: rgb(255, 102, 0, 0.6);
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
