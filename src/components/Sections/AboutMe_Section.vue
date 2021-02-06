<template>
  <b-container fluid class="resumeWrapper">
    <b-row>
      <b-col class="col">
        <img src="@/assets/resumeImage.png" alt="Titel Image" id="titelImg">
      </b-col>
      <b-col class="col">
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
          <b-tabs content-class="mt-3">
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
.col{
  width: 100%;
  height: 100vh;
  background-color: #3e5a79;
}
#resumeCard{
  width: 100%;
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
    background-color: #fd7e35;
    color: black;
    font-weight: bold;
    font-size: 20px;
}
.listItem{
    font-weight: bold;
    font-size: 20px;
    color: white;
    background-color: transparent;
}
</style>
