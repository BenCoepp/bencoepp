<template>
  <vue-scroll-snap>
    <Titel_Section class="item"/>
    <WhatIDo_Section class="item"/>
    <Resume_Section class="item"/>
    <b-container fluid>
      <AGuidetoQt6_Project msg="Project 1" class="item"/>
      <Cherry_Project msg="Project 2" class="item"/>
    </b-container>
    <Disclaimer msg="Welcome to Your Vue.js App" class="item"/>
    <Contact_Section msg="Welcome to Your Vue.js App" class="item"/>
  </vue-scroll-snap>
</template>

<script>
// @ is an alias to /src
import VueScrollSnap from "vue-scroll-snap";
import Titel_Section from "@/components/Sections/Titel_Section.vue";
import WhatIDo_Section from "@/components/Sections/WhatIDo_Section.vue";
import Resume_Section from "@/components/Sections/Resume_Section.vue";
import Contact_Section from "@/components/Sections/Contact_Section.vue";
import Disclaimer from "@/components/Disclaimer.vue";

import AGuidetoQt6_Project from "@/components/Projects/AGuidetoQt6_Project.vue";
import Cherry_Project from "@/components/Projects/Cherry_Project.vue";
export default {
  name: "Home",
  components: {
    VueScrollSnap,
    Titel_Section,
    WhatIDo_Section,
    Resume_Section,
    Contact_Section,
    Disclaimer,
    AGuidetoQt6_Project,
    Cherry_Project
  }
};
</script>
<style>
.scroll-snap-container {
  height: 100vh;
  width: 100%;
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}
.scroll-snap-container::-webkit-scrollbar {
  display: none;
}
.item {
  /* Set the minimum height of the items to be the same as the height of the scroll-snap-container.*/
  min-height: 100vh;
}
</style>
