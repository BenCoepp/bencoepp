<template>
  <fixed-header>
    <div class="navbar">
      Your Content
    </div>
  </fixed-header>
</template>

<script>
import FixedHeader from 'vue-fixed-header'

export default {
  name: "Nav",
  components: {
    FixedHeader
  },
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.navbar.vue-fixed-header--isFixed {
  position: fixed;
  left: 0;
  top: 0;
  width: 100vw;
}
.navbar{
  background-color: #3e5a79;
}
</style>
