<template>
  <div class="home">
    <Titel_Section msg="Welcome to Your Vue.js App" />
    <WhatIDo_Section msg="Welcome to Your Vue.js App" />
    <Resume_Section msg="Welcome to Your Vue.js App" />
    <b-container fluid>
      <AGuidetoQt6_Project msg="Project 1" />
      <Cherry_Project msg="Project 2" />
    </b-container>
    <Disclaimer msg="Welcome to Your Vue.js App" />
    <Contact_Section msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
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
