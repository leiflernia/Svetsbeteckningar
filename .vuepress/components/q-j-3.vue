<template>
  <div>
    <input type="radio" id="pill" value="Nej, försök igen" v-model="picked" />
    <label for="pill">Pillinje</label>
    <br />
    <input type="radio" id="hanl" value="Det var fel" v-model="picked" />
    <label for="hanl">Hänvisningslinje</label>
    <br />
    <input type="radio" id="undl" value="Rätt" v-model="picked" />
    <label for="undl">Underreferenslinje</label>
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