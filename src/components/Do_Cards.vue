<template>
  <b-card 
    title="{this.titel}"
    img-src="https://picsum.photos/600/300/?image=25"
    img-alt="Image"
    img-top
    id="doCard"
    >
    <b-card-text>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. 
        Rem quae velit dolores rerum, facilis accusantium laudantium! 
        Recusandae, amet molestias autem eaque neque ratione porro 
        id rerum illum. Dolor, sed ea.
    </b-card-text>
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
