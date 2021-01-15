<template>
  <div>
    <input type="radio" id="pil" value="Rätt" v-model="picked" />
    <label for="pil">Pilsidan</label>
    <br />
    <input type="radio" id="andra" value="Det var fel" v-model="picked" />
    <label for="andra">Andra sidan</label>
    <br />
    <input type="radio" id="framre" value="Nej, försök igen" v-model="picked" />
    <label for="framre">Främre sidan</label>
    <br />
    <br />
    <span>Svar: {{ picked }}</span>
  </div>
</template>

<script>
export default {
  props: ['picked']
}
</script>

<style scoped>
div {
  margin-top: 1rem;
}
label {
  padding: 0.2rem;
}
</style>