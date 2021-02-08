<template>
  <b-navbar toggleable="lg" type="dark" class="nav">
    <b-navbar-brand href="#" id="brandTitel">
      <img src="@/assets/logo.png" class="d-inline-block align-top" alt="Logo Ben Coepp" id="logo">
      <router-link to="/" id="brandTitel">Ben Coepp</router-link>
    </b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <router-link to="/mystuff" class="rLink">My Stuff</router-link>
        <router-link to="/mystuff" class="rLink">Products</router-link>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>

export default {
  name: "Nav",
  components: {
  },
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.nav{
  background-color: #3e5a79;
}
#brandTitel{
  font-weight: bold;
  color: white;
  margin-left: 10px;
}
#brandTitel:hover{
  color: #fd7e35;
  text-decoration: none;
}
.rLink{
  margin-right: 1em;
  color: white;
}
.rLink:hover{
  text-decoration: none;
  color: #fd7e35;
}
#logo{
  width: 35px;
}
</style>
