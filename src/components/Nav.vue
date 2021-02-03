<template>
  <b-navbar toggleable="lg" type="dark" class="nav">
    <b-navbar-brand href="#" id="brandTitel">
      <img src="https://placekitten.com/g/30/30" class="d-inline-block align-top" alt="Kitten">
      <router-link to="/" class="rLink">Ben Coepp</router-link>
    </b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <router-link to="/about" class="rLink">My Stuff</router-link>
        <router-link to="/about" class="rLink">Products</router-link>
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
}
#brandTitel:hover{
  color: #fd7e35;
}
.rLink{
  margin-right: 1em;
  color: white;
}
.rLink:hover{
  text-decoration: none;
  color: #fd7e35;
}
</style>
