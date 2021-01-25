<template>
  <b-container fluid class="disclaimerWrapper">

  </b-container>
</template>

<script>
export default {
  name: "Disclaimer",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.disclaimerWrapper{
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
}
</style>
