<template>
  <b-container fluid class="contactWrapper">
    <b-row>
      <b-col>
        <b-row>
          <h1>Let's get in touch</h1>
          <h2>You can contact me when ever you want just go ahead</h2>
        </b-row>
        <b-row>
          <b-col id="telCardCol">
             <b-card class="telCard">
              <b-icon-telephone id="telCardIcon"></b-icon-telephone>
              <b-card-text>Please only use when contacting for buying reasons</b-card-text>
              <b-card-text>0173 4066728</b-card-text>
            </b-card>
            <b-card class="telCard">
              <b-icon-text-left id="telCardIcon"></b-icon-text-left>
              <b-card-text>Please only use when contacting for buying reasons</b-card-text>
              <b-card-text>0173 4066728</b-card-text>
            </b-card>
            <b-card class="telCard">
              <b-icon-emoji-sunglasses id="telCardIcon"></b-icon-emoji-sunglasses>
              <b-card-text>Please only use when contacting for buying reasons</b-card-text>
              <b-card-text>0173 4066728</b-card-text>
            </b-card>
          </b-col>
        </b-row>
        <b-icon-triangle-fill rotate="-90" id="arrawIcon"></b-icon-triangle-fill>
      </b-col>
      <b-col id="rightColContact">
         <b-icon-triangle-fill rotate="-90" id="arrawIcon"></b-icon-triangle-fill>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Contact_Section",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.contactWrapper{
  height: 100vh;
  background-color: #3e5a79;
  margin: 0;
}
#telCardCol{
  margin: 10%;
}
.telCard{
  float: right;
  margin-bottom: 1em;
  width: 60%;
  background-color: #3e5a79;
  color: white;
  -webkit-box-shadow: 5px 5px 19px 7px rgba(62,90,121,0.82); 
  box-shadow: 5px 5px 19px 7px rgba(62,90,121,0.82);
}
#telCardIcon{
  width: 40px;
  height: 40px;
  color: white;
}
#rightColContact{
  background-color: #fd7e35;
  height: 100vh;
}
#arrawIcon{
  width: 60px;
  height: 60px;
  position: absolute;
  top: 10%;
  left: 96%;
  color: #fd7e35;
}
</style>
