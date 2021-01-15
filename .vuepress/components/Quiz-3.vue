<template>
  <div>
    <input type="radio" id="bortre" value="Det var fel" v-model="picked" />
    <label for="bortre">Bortre sidan</label>
    <br />
    <input type="radio" id="andras" value="Rätt" v-model="picked" />
    <label for="andras">Andra sidan</label>
    <br />
    <input type="radio" id="forsta" value="Nej, försök igen" v-model="picked" />
    <label for="forsta">Främre sidan</label>
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