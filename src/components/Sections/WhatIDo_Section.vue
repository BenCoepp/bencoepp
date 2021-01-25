<template>
  <b-container fluid class="doWrapper">
    <b-row>
      <b-col class="col">
        <b-col id="cardCol">
          <b-col><Do_Cards id="myCard1"/></b-col>
          <b-col><Do_Cards id="myCard2"/></b-col>
          <b-col><Do_Cards id="myCard3"/></b-col>
        </b-col>
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
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Vel dolor in repellendus pariatur totam facere, 
            magni repellat debitis odit maxime, rerum quisquam 
            nam delectus qui quos molestias perspiciatis, 
            perferendis quas.
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
  width: 90%;
  height: 20%;
  margin-bottom: 1em;
}
#myCard2{
  width: 90%;
  height: 20%;
  margin-bottom: 1em;
}
#myCard3{
  width: 90%;
  height: 20%;
  margin-bottom: 1em;
}
#cardCol{
  margin: 15%;
}
</style>
