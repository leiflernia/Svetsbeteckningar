<template>
  <div>
    <input type="radio" id="V" value="Rätt" v-model="picked" />
    <label for="V">Halv V-fog</label>
    <br />
    <input type="radio" id="Y" value="Det var fel" v-model="picked" />
    <label for="Y">Halv Y-fog</label>
    <br />
    <input type="radio" id="J" value="Nej, försök igen" v-model="picked" />
    <label for="J">J-fog</label>
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