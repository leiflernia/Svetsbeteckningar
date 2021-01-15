<template>
  <div>
    <input type="radio" id="q4andra" value="Rätt" v-model="picked" />
    <label for="q4andra">Andra sidan</label>
    <br />
    <input type="radio" id="q4bak" value="Det var fel" v-model="picked" />
    <label for="q4bak">Baksidan</label>
    <br />
    <input type="radio" id="q4pil" value="Nej, försök igen" v-model="picked" />
    <label for="q4pil">Pilsidan</label>
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