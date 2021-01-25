<template>
  <b-card 
    title="{this.titel}"
    id="doCard"
    >
    <b-card-text>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. 
        Rem quae velit dolores rerum, facilis accusantium laudantium! 
        Recusandae, amet molestias autem eaque neque ratione porro 
    </b-card-text>
    <b-avatar src="https://placekitten.com/300/300"></b-avatar>
    <b-badge id="b1">Quality 1</b-badge>
    <b-badge id="b2">Quality 1</b-badge>
    <b-badge id="b3">Quality 1</b-badge>
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
#b1{
  background-color: orange;
  font-size: 20px;
  display: inline-flex;
  margin-left: 10px;
}
#b2{
  background-color: red;
  font-size: 20px;
  display: inline-flex;
  margin-left: 10px;
}
#b3{
  background-color: blue;
  font-size: 20px;
  display: inline-flex;
  margin-left: 10px;
}
</style>
