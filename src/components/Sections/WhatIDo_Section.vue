<template>
  <b-container fluid class="doWrapper">
    <b-row>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <b-col id="cardCol">
          <b-col><Do_Cards id="myCard1" 
            titelD="Developer"
            quality1="Dedicated"
            quality2="Bug-Hunter"
            quality3="Relentless"
            text="I am a Developer at heart, I code nearly every day, 
            and try to spend as much time as possible working on applications."
          /></b-col>
          <b-col><Do_Cards id="myCard2" 
            titelD="Writer"
            quality1="Pacionat"
            quality2="Open-Minded"
            quality3="Happy"
            text="I write books, about Coding, Development and the Life of a
            Software Engenier, you want get bored reading what I write."
          /></b-col>
          <b-col><Do_Cards id="myCard3" 
            titelD="YouTuber"
            quality1="Outgoing"
            quality2="Master of Procrasination"
            quality3="Techi"
            text="Not a lot of Subscripers but thats not why I am doing this, 
            from Tutoirals to Reviews there will be something for you. "
          /></b-col>
        </b-col>
      </b-col>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <b-card
          tag="article"
          class="mb-2"
          id="titelCard"
        >
          <b-card-text id="titel1">What</b-card-text>
          <b-card-text id="titel2">I DO</b-card-text>
          <b-card-text id="titelText">
            Well, a lot from time to time, as you can see, I am a Developer, 
            Writer and a YouTuber. So, yes I do a lot, and maybe throw some
            what I do you found this Website. If so hope you like it, scroll
            around and find out who I am and what I do.
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
@media only screen and (min-width: 600px) {
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
  width: 85%;
  height: 20%;
  margin-bottom: 1em;
  border-color: white;
}
#myCard2{
  width: 85%;
  height: 20%;
  margin-bottom: 1em;
}
#myCard3{
  width: 85%;
  height: 20%;
  margin-bottom: 1em;
  border-color: white;
}
#cardCol{
  margin: 15%;
}
}
@media only screen and (max-width: 600px) {
.doWrapper{
  width: 100%;
  padding-bottom: 8em;
  background-color: #3e5a79;
}
#titelCard{
background-color: transparent;
border: 0;
padding-bottom: 2em;
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
#myCard1{
  margin-bottom: 1em;
}
#myCard2{
  margin-bottom: 1em;
}
#myCard3{
  margin-bottom: 1em;
}
}
</style>
