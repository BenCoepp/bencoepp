<template>
  <b-container fluid class="disclaimerWrapper">
    <b-row>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <b-card
          tag="article"
          class="mb-2"
          id="resumeCard"
        >
          <b-card-text id="titel1">A</b-card-text>
          <b-card-text id="titel2">DISCLAIMER</b-card-text>
          <b-card-text id="titelText">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Vel dolor in repellendus pariatur totam facere, 
            magni repellat debitis odit maxime, rerum quisquam 
            nam delectus qui quos molestias perspiciatis, 
            perferendis quas.
          </b-card-text>
        </b-card>
      </b-col>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <b-col id="cardCol">
          <b-col><Do_Cards id="myCard1"
            titelD="Can you hire me?"
            quality1="Sorry,"
            quality2="No,"
            quality3="Unfortanatly"
            text="If you were looking to hire me for a Job, then I am sorry to 
            inform you that I am currently under contract. This means that I
            can not work for you. A Man can only know one Master. But you can 
            still contact me consurning help, or if it is about a contract you 
            want me to do."
          /></b-col>
          <b-col><Do_Cards id="myCard2"
            titelD="What is this all for?"
            quality1="Who am I"
            quality2="My Work"
            quality3="My Stuff"
            text="The porpuse of this Website is to show you who I am, what
            I do, and sell. I hope you you were able to find out a few things
            about me. Also try to check out all the other things I do.
            My mission is to educate and inform you about how to be a Developer,
            there are a few ways to do this, but I hope I know the right one."
          /></b-col>
        </b-col>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Do_Cards from "@/components/Do_Cards.vue";
export default {
  name: "Disclaimer",
  props: {
    msg: String
  },
  components:{
    Do_Cards
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@media only screen and (min-width: 600px) {
.disclaimerWrapper{
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
}
#resumeCard{
  width: 60%;
  margin: 20%;
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
#cardCol{
  margin-top: 20%;
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
}
@media only screen and (max-width: 600px) {
.disclaimerWrapper{
  padding-bottom: 8em;
  background-color: #3e5a79;
  margin: 0;
}
#resumeCard{
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
}
#myCard1{
  margin-bottom: 1em;
}
#myCard2{
  margin-bottom: 1em;
}
</style>
