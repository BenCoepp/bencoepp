<template>
  <b-container fluid class="navWrapper">
    <b-avatar src="https://placekitten.com/300/300" id="logo"></b-avatar>
    <h2 id="companyName">Ben Coepp</h2>
    <router-link class="routerLink" to="/">Portfolio</router-link>
    <router-link class="routerLink" to="/about">My Stuff</router-link>
    <router-link class="routerLink" to="/products">Products</router-link>
  </b-container>
</template>

<script>
export default {
  name: "Disclaimer",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.navWrapper{
  width: 100%;
  background-color: #fd7e35;
  height: 50px;
  display: inline-flex;
}
#logo{
    margin: 3px;
}
#companyName{
    font-weight: bold;
    color: white;
    margin-left: 10px;
}
.routerLink{
    margin-top: 10px;
    margin-left: 1em;
    font-weight: bold;
    color: white;
}
</style>
