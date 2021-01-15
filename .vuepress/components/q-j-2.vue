<template>
  <div>
    <input type="radio" id="rl" value="Nej, försök igen" v-model="picked" />
    <label for="rl">Referanslinje</label>
    <br />
    <input type="radio" id="pl" value="Det var fel" v-model="picked" />
    <label for="pl">Pillinje</label>
    <br />
    <input type="radio" id="hl" value="Rätt" v-model="picked" />
    <label for="hl">Hänvisningslinje</label>
    <br />
    <br />
    <span>Svar: {{ picked }}</span>
  </div>
</template>

<script>
export default {
  props: ["picked"],
};
</script>

<style scoped>
div {
  margin-top: 1rem;
}
label {
  padding: 0.2rem;
}
</style>