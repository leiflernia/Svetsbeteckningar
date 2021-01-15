<template>
  <div>
    <div style="display: flex; align-items: center">
      <div> <input type="radio" id="y1" value="Rätt" v-model="picked" /></div>
      <div><label for="y1"><img style="margin-bottom: 0" src="yq1b1.jpg" /></label></div>
    </div>
    <br />
    <div style="display: flex; align-items: center">
      <div><input type="radio" id="y2" value="Det var fel" v-model="picked" /></div>
      <div><label for="y2"><img style="margin-bottom: 0" src="yq1b2.jpg" /></label></label></div>
    </div>
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