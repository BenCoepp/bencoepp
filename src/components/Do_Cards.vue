<template>
  <b-card 
    id="doCard"
    >
    <b-card-text id="titel">{{titelD}}</b-card-text>
    <b-card-text id="text">{{text}}</b-card-text>
    <b-badge id="b1">{{quality1}}</b-badge>
    <b-badge id="b2">{{quality2}}</b-badge>
    <b-badge id="b3">{{quality3}}</b-badge>
  </b-card>
</template>

<script>
export default {
  name: "Do_Card",
  props:{
      titelD: String,
      quality1: String,
      quality2: String,
      quality3: String,
      text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#b1{
  background-color: #a1c181;
  color: black;
  font-size: 20px;
  display: inline-flex;
  margin-right: 10px;
}
#b2{
  background-color: #78d5e3;
  color: black;
  font-size: 20px;
  display: inline-flex;
  margin-right: 10px;
}
#b3{
  background-color: #b493a5;
  color: black;
  font-size: 20px;
  display: inline-flex;
  margin-right: 10px;
}
#titel{
  font-weight: bold;
  color: black;
  font-size: 35px;
  margin-bottom: 0;
}
#text{
  font-size: 16px;
}
</style>
