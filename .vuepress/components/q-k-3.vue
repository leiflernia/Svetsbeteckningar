<template>
  <div>
    <input type="radio" id="AndS" value="Rätt" v-model="picked" />
    <label for="AndS">Andra sidan</label>
    <br />
    <input type="radio" id="BakS" value="Det var fel" v-model="picked" />
    <label for="BakS">Baksidan</label>
    <br />
    <input type="radio" id="FramS" value="Nej, försök igen" v-model="picked" />
    <label for="FramS">Framsidan</label>
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