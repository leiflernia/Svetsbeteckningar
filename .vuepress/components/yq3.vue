<template>
  <div>
    <input type="radio" id="svets" value="Nej, försök igen" v-model="picked" />
    <label for="svets">Svetssymbol</label>
    <br />
    <input type="radio" id="bas" value="Det var fel" v-model="picked" />
    <label for="bas">Bassymbol</label>
    <br />
    <input type="radio" id="grund" value="Rätt" v-model="picked" />
    <label for="grund">Grundsymbol</label>
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