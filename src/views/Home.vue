<template>
  <div>
    <img alt="Vue logo" src="../assets/gestform.png" />
    <div class="home">
      <Consignes />
      <Test />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Consignes from "@/components/Consignes.vue";
import Test from "@/components/Test.vue";

export default {
  name: "Home",
  components: {
    Consignes,
    Test,
  },
};
</script>

<style scoped>
img {
  max-width: 80%;
  margin-top: 70px;
  margin-bottom: 70px;
}
.home {
  display: flex;
}
@media (max-width: 1024px) {
  .home {
    flex-direction: column;
  }
}
</style>
