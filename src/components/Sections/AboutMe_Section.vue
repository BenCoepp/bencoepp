<template>
  <b-container fluid class="resumeWrapper">
    <b-row>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <img src="@/assets/aboutmeImage.png" alt="Titel Image" id="titelImg">
      </b-col>
      <b-col class="col-sm" id="col" sm="12" md="6">
        <b-card
          tag="article"
          class="mb-2"
          id="resumeCard"
        >
          <b-card-text id="titel2">About Me</b-card-text>
          <b-card-text id="titelText">
            Well as you are here, how about a few key facts about me. They
            reange from myself to school and the like to other things that
            you might find interesting so have a look.
          </b-card-text>
          <b-tabs content-class="mt-3"
          active-nav-item-class="font-weight-bold bg-white"
          active-tab-class="font-weight-bold"
          >
            <b-tab title="Personal"> 
                <b-list-group flush>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Name:
                        <b-badge class="pPill">Ben Cöppicus | Ben Coepp</b-badge>
                    </b-list-group-item>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Age:
                        <b-badge class="pPill">20</b-badge>
                    </b-list-group-item>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Country:
                        <b-badge class="pPill">Germany</b-badge>
                    </b-list-group-item>
                </b-list-group>
            </b-tab>
            <b-tab title="Skills">
                <b-list-group flush>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Java
                        <b-badge class="pPill">Intermediat</b-badge>
                    </b-list-group-item>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        HTML / CSS / JavaScript
                        <b-badge class="pPill">Intermediat</b-badge>
                    </b-list-group-item>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Qt
                        <b-badge class="pPill">Master</b-badge>
                    </b-list-group-item>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        C++
                        <b-badge class="pPill">Intermediat</b-badge>
                    </b-list-group-item>
                </b-list-group>
            </b-tab>
            <b-tab title="Education">
                <b-list-group flush>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Highschool | University :
                        <b-badge class="pPill">2011 - 2019</b-badge>
                    </b-list-group-item>
                    <b-list-group-item class="d-flex justify-content-between align-items-center listItem">
                        Apprenticeship :
                        <b-badge class="pPill">2020 - ????</b-badge>
                    </b-list-group-item>
                </b-list-group>
            </b-tab>
          </b-tabs>
          <b-card-text id="titelText">
            This might not satisfy your craving for information about me, but
            this needs to suffice. You can learn more about me, what I do and 
            what I sell on this website, you just need to keep searching for it.
          </b-card-text>
          <b-list-group horizontal>
            <b-list-group-item  class="listItem1">
              <b-link href="https://github.com/BenCoepp" target="blank" class="itemLink">
                <b-icon-github id="telCardIcon"></b-icon-github>
              </b-link>
            </b-list-group-item>
            <b-list-group-item  class="listItem1">
              <b-link href="https://www.instagram.com/ben.coepp" target="blank" class="itemLink">
                <b-icon-instagram id="telCardIcon"></b-icon-instagram>
              </b-link>
            </b-list-group-item>
            <b-list-group-item  class="listItem1">
              <b-link href="https://twitter.com/BCoepp" target="blank" class="itemLink">
                <b-icon-twitter id="telCardIcon"></b-icon-twitter>
              </b-link>
            </b-list-group-item>
            <b-list-group-item  class="listItem1">
              <b-link href="https://www.youtube.com/channel/UC7BNSmIzVZ9fnw3uMlLj_kw" target="blank" class="itemLink">
                <b-icon-youtube id="telCardIcon"></b-icon-youtube>
              </b-link>
            </b-list-group-item>
          </b-list-group>
          <b-card-text id="titelText">
            If you are interested you can also follow me on Twitter, Instagram,
            YouTube, and Git-Hub.
          </b-card-text>
        </b-card>
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
#resumeCard{
  width: 90%;
  margin: 2%;
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
.pPill{
    background-color: white;
    color: black;
    font-weight: bold;
    font-size: 20px;
}
.listItem{
    font-weight: bold;
    font-size: 20px;
    color: #fd7e35;
    background-color: transparent;
}
.listItem1{
    font-weight: bold;
    font-size: 30px;
    background-color: transparent;
    border: 0;
}
.itemLink{
  color: #fd7e35;
}
}
@media only screen and (max-width: 600px) {
.resumeWrapper{
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
  padding-bottom: 8em;
}
#titelImg{
  display: none;
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
.pPill{
    background-color: white;
    color: black;
    font-weight: bold;
    font-size: 15px;
}
.listItem{
    font-weight: bold;
    font-size: 15px;
    color: #fd7e35;
    background-color: transparent;
}
.listItem1{
    font-weight: bold;
    font-size: 15px;
    background-color: transparent;
    border: 0;
}
.itemLink{
  color: #fd7e35;
}
}
</style>
