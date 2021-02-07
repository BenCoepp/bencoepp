<template>
  <b-container fluid class="projectWrapper">
    <b-row>
      <b-col cols="8" class="col">
        <b-row id="rightCol">
          <b-card
            tag="article"
            class="mb-2"
            id="titelCard"
          >
            <b-card-text id="titel1">A Guide to Qt 6</b-card-text>
            <b-card-text id="titel2">A Beginner's Guide to Qt</b-card-text>
            <b-card-text id="titelText">
              Well, a lot from time to time, as you can see, I am a Developer, 
              Writer and a YouTuber. So, yes I do a lot, and maybe throw some
              what I do you found this Website. If so hope you like it, scroll
              around and find out who I am and what I do.
            </b-card-text>
            <b-button-group id="buttonBox">
              <b-button id="buyBt">
                <a target="blank" id="downloadResumeBt" href="https://firebasestorage.googleapis.com/v0/b/ben-coepp.appspot.com/o/Lebenslauf.pdf?alt=media&token=58a18c73-5b18-40f0-85c5-4491d3a8f272">Buy</a>
              </b-button>
              <b-button id="learnMoreBt" v-b-modal.learnMoreModel>Learn More</b-button>
            </b-button-group>
            <b-modal id="learnMoreModel" title="Q Guide to Qt 6">
              <p class="my-4">Hello from modal!</p>
            </b-modal>
            <b-card-text id="titelText">
              Well, a lot from time to time, as you can see, I am a Developer, 
              Writer and a YouTuber. So, yes I do a lot, and maybe throw some
              what I do you found this Website. If so hope you like it, scroll
              around and find out who I am and what I do.
            </b-card-text>
            <b-card-text id="titelText">
              Well, a lot from time to time, as you can see, I am a Developer, 
              Writer and a YouTuber. So, yes I do a lot, and maybe throw some
              what I do you found this Website. If so hope you like it, scroll
              around and find out who I am and what I do.
            </b-card-text>
            <b-badge class="badge" id="badge1">Developer</b-badge>
            <b-badge class="badge" id="badge2">Writer</b-badge>
            <b-badge class="badge" id="badge3">YouTuber</b-badge>
          </b-card>
        </b-row>
      </b-col>
      <b-col cols="4" class="col">
        <b-row id="leftCol">
          <img src="@/assets/guidetoqt6Cover.png" alt="Project Image" id="projectImg">
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Project 1",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.projectWrapper{
  width: 100%;
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
  padding: 0;
}
.col{
  width: 100%;
  height: 100vh;
  margin: 0;
  padding: 0;
}
#leftCol{
  width: 100%;
  height: 100vh;
}
#projectImg{
  margin: auto;
  margin-top: 15%;
  display: block;
  height: 65%;
}
#titelCard{
  width: 90%;
  margin: 5%;
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
  font-size: 35px;
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

#downloadResumeBt{
  background-color: #FD7E35;
  width: 150px;
  color: black;
  font-weight: bold;
  font-size: 20px;
  text-decoration: none;
}
#buyBt{
  background-color: #FD7E35;
  width: 150px;
  color: black;
  font-weight: bold;
  font-size: 20px;
  margin-right: 1em;
}
#learnMoreBt{
  background-color: #FD7E35;
  width: 150px;
  color: black;
  font-weight: bold;
  font-size: 20px;
  margin-right: 1em;
}
#buttonBox{
  display: inline-flex;
}
</style>
