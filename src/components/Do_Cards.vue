<template>
  <b-card
    title="Card Title"
    img-src="https://picsum.photos/600/300/?image=25"
    img-alt="Image"
    img-top
    id="doCard"
  >
  </b-card>
</template>

<script>
export default {
  name: "Do_Card",
  props:{
      titel: String,
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
