<template>
  <div>
    <input type="radio" id="J" value="Rätt" v-model="picked" />
    <label for="J">J-fog</label>
    <br />
    <input type="radio" id="hY" value="Det var fel" v-model="picked" />
    <label for="hY">Halv Y-fog</label>
    <br />
    <input type="radio" id="hV" value="Nej, försök igen" v-model="picked" />
    <label for="hV">Halv V-fog</label>
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