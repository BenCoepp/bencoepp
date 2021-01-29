<template>
  <b-navbar toggleable="lg" type="dark" class="nav">
    <b-navbar-brand href="#" id="brandTitel">
      <img src="https://placekitten.com/g/30/30" class="d-inline-block align-top" alt="Kitten">
      Ben Coepp
    </b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <router-link to="/about">About</router-link>
        <b-nav-item href="#" disabled>Disabled</b-nav-item>
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
</style>
