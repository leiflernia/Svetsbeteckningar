<template>
  <div>
    <div style="display: flex; align-items: center">
      <div> <input type="radio" id="y21" value="Rätt" v-model="picked" /></div>
      <div><label for="y21"><img style="margin-bottom: 0" src="yq2b1.jpg" /></label></div>
    </div>
    <br />
    <div style="display: flex; align-items: center">
      <div><input type="radio" id="y22" value="Det var fel" v-model="picked" /></div>
      <div><label for="y22"><img style="margin-bottom: 0" src="yq2b2.jpg" /></label></label></div>
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