<template>
  <b-container fluid class="projectWrapper">
    <b-row>
      <b-col class="col-sm" id="col" sm="12" md="8">
        <b-row id="rightCol">
          <b-card
            tag="article"
            class="mb-2"
            id="titelCard"
          >
            <b-card-text id="titel1">A Guide to Qt 6 
              <b-button-group id="buttonBox">
                <b-button id="buyBt">
                  <a target="blank" id="downloadResumeBt" href="https://firebasestorage.googleapis.com/v0/b/ben-coepp.appspot.com/o/Lebenslauf.pdf?alt=media&token=58a18c73-5b18-40f0-85c5-4491d3a8f272">Buy</a>
                </b-button>
              </b-button-group>
            </b-card-text>
            <b-card-text id="titel2">A Beginner's Guide to Qt</b-card-text>
            <b-card-text id="titelText">
              This is my first educational book, it is about learning to use Qt. 
              Qt is a C++ Framework with which you can create Desktop and Mobile
              Applications. It is extremly fast, resource freindly and the 
              Applications you build will run on every platform on the planet. 
            </b-card-text>
            <b-modal id="learnMoreModel" title="Q Guide to Qt 6">
                <h6>
                  Ever wanted to create your own Desktop, or Mobile Applciations? 
                  Well than you propbely searched around on Google on what 
                  Frameworks, and Tools exist with which you can do this.
                  And there you probebly stumbled apon Qt, it is one of the best 
                  Frameworks for creating Desktop and Mobile Applications.
                </h6>
                <h6>
                  Unfortanatly thow there are not a lot of Tutorials, Videos or 
                  Books about Qt. And because Qt 6 released a few Weeks ago, 
                  it is the perfect Time to grap this Book and start learning 
                  about the Things you can to with Qt. In this Book you will 
                  learn everything about:
                </h6>
                <ul>
                  <li>- Creating your own Appications</li>
                  <li>- Building and Publishing them</li>
                  <li>- Deploying Applciations on Mobile Devices</li>
                  <li>Learn how to use all of the Components Qt has to offer, like</li>
                  <li>- Grid- / ListViews and Models</li>
                  <li>- Stack- / SwipeViews</li>
                  <li>- MouseAreas and Buttons</li>
                  <li>- How to best work with large Projects and complicated Desings</li>
                  <li>- Advanced Topics like Git, Charts and Custom Components</li>
                </ul>
                <h6>
                  And a lot more, I will take you throw a few Applications which 
                  we will build from Start to finish together. From the Project 
                  Creation, to the actuall Coding and finally the building and 
                  Deploying of our Application on our desiered Platform.
                </h6>
            </b-modal>
            <b-card-text id="titelText">
              As this is an educationanal book, it focuses on teaching you how to 
              use Qt, how to set it up for Mobile and Desktop Development and how 
              to make applciations for both. You can click <b-link id="featureList" v-b-modal.learnMoreModel>here</b-link>
              to learn more about what I will teach you in the Book, but for You
              a little sneak peak:
            </b-card-text>
            <ul id="featureList">
              <li>- Basic QML Components</li>
              <li>- Qt Charts</li>
              <li>- C++ Integration into QML Quick Applications</li>
              <li>- Mobile and Desktop Development</li>
            </ul>
            <b-card-text id="titelText">
              As you can see there are a few things I will teach you and a lot more.
              Go check it out, and leave give me your feedback how it was. 
            </b-card-text>
            <AGuidetoQt6_ProblemModal/>
            <b-badge class="badge" id="badge1">Educational</b-badge>
            <b-badge class="badge" id="badge2">Tutorial</b-badge>
            <b-badge class="badge" id="badge3">Qt</b-badge>
          </b-card>
        </b-row>
      </b-col>
      <b-col class="col-sm" id="col" sm="12" md="4">
        <b-row id="leftCol">
          <img src="@/assets/guidetoqt6Cover.png" alt="Project Image" id="projectImg">
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import AGuidetoQt6_ProblemModal from './AGuidetoQt6_ProblemModal.vue'
export default {
  name: "Project 1",
  components:{
    AGuidetoQt6_ProblemModal
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@media only screen and (min-width: 600px) {
.projectWrapper{
  width: 100%;
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
  padding: 0;
}
#col{
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
  width: 70%;
  margin: 5%;
  margin-left: 13%;
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
  margin-left: 1em;
}
#featureList{
  color: #FD7E35;
  font-weight: bold;
  font-size: 16px;
  text-decoration: none;
}
}
@media only screen and (max-width: 600px) {
  .projectWrapper{
  width: 100%;
  background-color: #3e5a79;
  margin: 0;
  padding-bottom: 8em;
}
#projectImg{
  margin: auto;
  display: block;
}
#titelCard{
  background-color: transparent;
  border: 0;
}
#titel1{
  margin-bottom: 0;
  font-size: 35px;
  font-weight: bold;
  color: white;
}
#titel2{
  font-size: 30px;
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
  color: black;
  font-weight: bold;
  font-size: 15px;
  text-decoration: none;
}
#buyBt{
  background-color: #FD7E35;
  width: 100px;
  color: black;
  font-weight: bold;
  font-size: 15px;
}
#learnMoreBt{
  background-color: #FD7E35;
  width: 150px;
  color: black;
  font-weight: bold;
  font-size: 20px;
}
#buttonBox{
  display: inline-flex;
}
#featureList{
  color: #FD7E35;
  font-weight: bold;
  font-size: 16px;
  text-decoration: none;
}
}
</style>
