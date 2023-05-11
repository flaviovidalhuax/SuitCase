<script setup>
import Navbar from "./components/Navbar.vue";
import Slider from "./components/Slider.vue";
import Banner from "./components/Banner.vue";
import Banner2 from "./components/Banner2.vue";
import SliderBag from "./components/SliderBag.vue";
import SliderBag2 from "./components/Sliderbag2.vue";
import Img from "./components/Img.vue";

import FooterPage from "./components/FooterPage.vue";
import Contact from "./components/Contact.vue";
import ButtonWA from "./components/ButtonWA.vue";
import Skill from "./components/SkillAt.vue";
</script>

<template>
  <v-app class="bg-app m-0 p-0">
    <Navbar></Navbar>
    <Contact id="aboutus"></Contact>
    <Banner  />
    <Slider :wa="whatsapp" id="experience"/>
      <div>
        <h3 class="text-white d-flex justify-center ">Experience Front end  </h3>
      </div>
    <SliderBag />
      <div>
        <h3 class="text-white d-flex justify-center ">Experience Back end  </h3>
      </div>
    <SliderBag2 />
    <Skill/>
    <FooterPage id="footer" />
    <ButtonWA></ButtonWA>
  </v-app>
</template>
    
<script>
export default {

  data() {
    return {
      whatsapp: "https://web.whatsapp.com/",
    };
  },
};
</script>

<style scoped>
</style>