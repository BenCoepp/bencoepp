<template>
  <div id="app">
    <vue-headful
      title="Ben Coepp"
      description="Ben Coepp - Portfolio"
      image="@/assets/logo.png"
    />
    <Nav/>
    <router-view />
  </div>
</template>
<script>
import Nav from "@/components/Nav.vue";
import vueHeadful from 'vue-headful';
export default {
  components:{
    Nav,
    vueHeadful
  }
}
</script>
<style lang="scss">
*{
  margin: 0;
  padding: 0;
  overflow: hidden; /* Hide scrollbars */
}

</style>
