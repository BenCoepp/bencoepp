<template>
  <b-container fluid class="doWrapper">
    <b-row>
      <b-col class="col">
        <Do_Cards id="myCard1"/>
        <Do_Cards id="myCard2"/>
        <Do_Cards id="myCard1"/>
      </b-col>
      <b-col class="col">
        <b-card
          tag="article"
          class="mb-2"
          id="titelCard"
        >
          <b-card-text id="titel1">What</b-card-text>
          <b-card-text id="titel2">I DO</b-card-text>
          <b-card-text id="titelText">
            Hello there on my Portfolio, I hope you will find anything interesting here.
            You can find my books, tutorials and projects here so do not hesitate and jump right in.
            Also if you want to contact me go ahead. 
          </b-card-text>
        </b-card>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Do_Cards from "@/components/Do_Cards.vue";
export default {
  name: "Titel_Section",
  components:{
    Do_Cards
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.doWrapper{
  width: 100%;
  height: 100vh;
  background-color: #3e5a79;
}
#titelCard{
  width: 70%;
  margin: 15%;
  background-color: transparent;
  border: 0;
}
#titel1{
  margin-bottom: 0;
  font-size: 60px;
  font-weight: bold;
  color: white;
}
#titel2{
  font-size: 70px;
  font-weight: bolder;
  color: #fd7e35;
}
#titelText{
  color: white;
  font-weight: bold;
}
#myCard1{
  width: 35%;
  height: 50%;
  position: absolute;
  top: 10%;
  left: 30%;
}
#myCard2{
  width: 35%;
  height: 50%;
  position: absolute;
  top: 50%;
  left: 55%;
  z-index: 1;
}
</style>
