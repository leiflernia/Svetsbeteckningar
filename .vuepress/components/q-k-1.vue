<template>
  <div>
    <input type="radio" id="U" value="Det var fel" v-model="picked" />
    <label for="U">U-fog</label>
    <br />
    <input type="radio" id="K" value="Rätt" v-model="picked" />
    <label for="K">Kälfog</label>
    <br />
    <input type="radio" id="Y" value="Nej, försök igen" v-model="picked" />
    <label for="Y">Y-fog</label>
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