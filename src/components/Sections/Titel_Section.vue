<template>
  <b-container fluid class="titelWrapper">
    <b-row>
      <b-col class="col-sm" id="col" sm="12" md="6">
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
      <b-col class="col-sm" id="col" sm="12" md="6">
        <img src="@/assets/titelImage.png" alt="Titel Image" id="titelImg">
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
@media only screen and (min-width: 600px) {
.titelWrapper{
  width: 100%;
  height: 100vh;
}
#col{
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
#badge1{background-color: #a1c181;}
#badge2{background-color: #78d5e3;}
#badge3{background-color: #b493a5;}

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
}
@media only screen and (max-width: 600px) {
.titelWrapper{
  width: 100%;
  padding-bottom: 8em;
  background-color: #3e5a79;
}
#col{
  width: 100%;
  background-color: #3e5a79;
}
#titelCard{
  background-color: transparent;
  border: 0;
}
#titel1{
  margin-bottom: 0;
  font-size: 30px;
  font-weight: bold;
  color: white;
}
#titel2{
  font-size: 35px;
  font-weight: bolder;
  color: #fd7e35;
}
#titelText{
  color: white;
  font-weight: bold;
}
.badge{
  font-size: 15px;
  margin-right: 1em;
}
#badge1{background-color: #a1c181;}
#badge2{background-color: #78d5e3;}
#badge3{background-color: #b493a5;}

#titelImg{
  width: 70%;
  margin-left: auto;
  margin-right: auto;
  display: block;
}
}
</style>
