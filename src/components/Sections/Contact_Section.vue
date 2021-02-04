<template>
  <b-container fluid class="contactWrapper">
    <b-row>
      <b-col>
        <b-row id="headRow">
          <h1 style="color: white; font-weight: bold; font-size: 55px">Let's get in touch</h1>
          <h3 style="color: white; font-weight: bold;">
            You can <h3 style="color: #fd7e35; display: inline-flex; font-weight: bold;">CONTACT ME</h3> 
            when ever you want just go ahead
          </h3>
        </b-row>
        <b-row>
          <b-col id="telCardCol">
             <b-card class="telCard">
              <b-icon-telephone id="telCardIcon"></b-icon-telephone>
              <b-card-text>Use this when you have extreme problems</b-card-text>
              <b-card-text>0173 4066728</b-card-text>
            </b-card>
            <b-card class="telCard">
              <b-icon-text-left id="telCardIcon"></b-icon-text-left>
              <b-card-text>Any question that you might have write me here</b-card-text>
              <b-card-text>bencoepp@gmail.com</b-card-text>
            </b-card>
            <b-card class="telCard">
              <b-icon-emoji-sunglasses id="telCardIcon"></b-icon-emoji-sunglasses>
              <b-card-text>Leave a Review here to show your support if you want</b-card-text>
              <b-card-text>AMAZON LINK</b-card-text>
            </b-card>
          </b-col>
        </b-row>
        <b-icon-triangle-fill rotate="-90" id="arrawIcon"></b-icon-triangle-fill>
      </b-col>
      <b-col id="rightColContact">
        <b-icon-triangle-fill rotate="-90" id="arrawIcon"></b-icon-triangle-fill>
        <Contact_Form/>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Contact_Form from '../Contact_Form'
export default {
  name: "Contact_Section",
  props: {
    msg: String
  },
  components:{
    Contact_Form
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
  margin: 5%;
}
.telCard{
  float: left;
  margin-bottom: 1em;
  background-color: #3e5a79;
  width: 70%;
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
#headRow{
  margin-top: 4%;
  margin-left: 5%;
  width: 75%;
}
</style>
