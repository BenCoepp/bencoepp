<template>
  <b-container fluid class="resumeWrapper">
    <b-row>
      <b-col>
        <b-card
          tag="article"
          class="mb-2"
          id="resumeCard"
        >
          <b-card-text id="titel1">My</b-card-text>
          <b-card-text id="titel2">Resume</b-card-text>
          <b-card-text id="titelText">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
            Vel dolor in repellendus pariatur totam facere, 
            magni repellat debitis odit maxime, rerum quisquam 
            nam delectus qui quos molestias perspiciatis, 
            perferendis quas.
          </b-card-text>
        </b-card>
      </b-col>
      <b-col col lg="4">
        <b-img src="@/assets/exampleImg.png" fluid alt="Responsive image" id="imgTitel"></b-img>
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
#imgTitel{
  margin-top: 10%;
  margin-bottom: 10%;
  width: 60%;
}
</style>
