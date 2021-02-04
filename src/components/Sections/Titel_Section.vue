<template>
  <b-container fluid class="titelWrapper">
    <b-row>
      <b-col class="col">
        <b-card
          tag="article"
          class="mb-2"
          id="titelCard"
        >
          <b-card-text id="titel1">HI I AM</b-card-text>
          <b-card-text id="titel2">Ben Cöppicus / BenCoepp</b-card-text>
          <b-card-text id="titelText">
            Hello there on my Portfolio, I hope you will find anything interesting here.
            You can find my books, tutorials and projects here so do not hesitate and jump right in.
            Also if you want to contact me go ahead. 
          </b-card-text>
          <b-badge class="badge" id="badge1">Developer</b-badge>
          <b-badge class="badge" id="badge2">Writer</b-badge>
          <b-badge class="badge" id="badge3">YouTuber</b-badge>
        </b-card>
      </b-col>
      <b-col class="col">
        <img src="@/assets/exampleImg.png" alt="Titel Image" id="titelImg">
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Titel_Section",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.titelWrapper{
  width: 100%;
  height: 100vh;
}
.col{
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
.badge{
  font-size: 20px;
  margin-right: 1em;
}
#badge1{background-color: #18BC9E;}
#badge2{background-color: #fd7e35;}
#badge3{background-color: #D23742;}

#imgTitel{
  margin-left: 20%;
  margin-right: 20%;
  margin-top: 10%;
  margin-bottom: 10%;
  width: 60%;
}
#titelImg{
  margin-left: auto;
  margin-right: auto;
  display: block;
  height: 80%;
}
</style>
