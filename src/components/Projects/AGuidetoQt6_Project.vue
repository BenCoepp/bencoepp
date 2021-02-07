<template>
  <b-container fluid class="projectWrapper">
    <b-row>
      <b-col cols="8" class="col">
        <b-row id="rightCol">

        </b-row>
      </b-col>
      <b-col cols="4" class="col">
        <b-row id="leftCol">
          <img src="@/assets/aboutmeImage.png" alt="Project Image" id="projectImg">
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
  background-color: #fd7e35;
}
#projectImg{
  width: 100%;
  height: 100%;
}
</style>
