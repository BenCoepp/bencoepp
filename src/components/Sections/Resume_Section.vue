<template>
  <b-container fluid class="resumeWrapper">
    <b-row>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <b-card
          tag="article"
          class="mb-2"
          id="resumeCard"
        >
          <b-card-text id="titel1">My</b-card-text>
          <b-card-text id="titel2">Resume</b-card-text>
          <b-card-text id="titelText">
            Want to know more about me? Well, here you can find my Resume, 
            what school did I go to, what do I know and what experience do
            I have. Because I am currently not for hire, this is not that
            important, but you might want to take a look at it, so here it is.
          </b-card-text>
          <b-button id="downloadResumeBt">
            <a target="blank" id="downloadResumeBt" href="https://firebasestorage.googleapis.com/v0/b/ben-coepp.appspot.com/o/Lebenslauf.pdf?alt=media&token=58a18c73-5b18-40f0-85c5-4491d3a8f272">Download</a>
          </b-button>
        </b-card>
      </b-col>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <img src="@/assets/resumeImage.png" alt="Titel Image" id="titelImg">
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Resume_Section",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@media only screen and (min-width: 600px) {
.resumeWrapper{
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
}
#resumeCard{
  width: 70%;
  margin: 12%;
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
#imgTitel{
  margin-top: 10%;
  margin-bottom: 10%;
  width: 60%;
}
#downloadResumeBt{
  background-color: #FD7E35;
  color: black;
  font-weight: bold;
  font-size: 20px;
  text-decoration: none;
}
#titelImg{
  margin-left: auto;
  margin-right: auto;
  display: block;
  height: 80%;
}
#col{
  width: 100%;
  height: 100vh;
  background-color: #3e5a79;
}
}
@media only screen and (max-width: 600px) {
.resumeWrapper{
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
}
#col{
  width: 100%;
  background-color: #3e5a79;
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
#titelImg{
  width: 70%;
  margin-left: auto;
  margin-right: auto;
  display: block;
}
#downloadResumeBt{
  background-color: #FD7E35;
  color: black;
  font-weight: bold;
  font-size: 20px;
  text-decoration: none;
}
}
</style>
