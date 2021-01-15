<template>
  <div>
    <input type="radio" id="PS" value="Rätt" v-model="picked" />
    <label for="PS">Pilsidan</label>
    <br />
    <input type="radio" id="AS" value="Det var fel" v-model="picked" />
    <label for="AS">Andra sidan</label>
    <br />
    <input type="radio" id="TS" value="Nej, försök igen" v-model="picked" />
    <label for="TS">Tredje sidan</label>
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