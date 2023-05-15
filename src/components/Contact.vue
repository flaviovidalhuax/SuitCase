<template>
  <v-row class="vh-85  py-5" id="contact">
      <v-col cols="6" class="p-0 d-md-flex">
        <v-img class="vh-85" :src="this.img" cover></v-img>
      </v-col>
      <v-col cols="6" class="bg-gray text-white p-0 overflow-hidden">
      <div class="d-flex flex-column justify-content-center align-items-center vh-85 gap-4 position-relative">
          <video :src="this.vid" 
              width="340"
              height="360"
              autoplay
              loop
              muted
              controls
              class="auto-content rounded-xl"
            ></video>
        <h2 class="fw-bolder">How I am</h2>
        <p class="px-5 mx-5 text-center">
          My name is Flavio Hernandez Jr. and I studied Electrical Engineering at UNAM, but I also took a Full Stack course in Javascript. For Front-end development, I am proficient in React.js, Node.js, and Vue.js. For Back-end development, I use Node.js. If you want to see my projects, you can check out my GitHub profile.
        </p>
        <v-col class="d-flex justify-content-center align-items-center">
          <v-btn id="btn" rounded="xl" variant="outlined" color="#754319" class="m-3 bg-white btnMove">
          <a
            :href="this.whatsapp"
            target="_blank"
            class="text-decoration-none text-black a-large "
          >
            <v-icon>mdi-whatsapp</v-icon>
            Contac me 
          </a>

          <a
            :href="this.whatsapp"
            target="_blank"
            class="text-decoration-none text-white a-small"
          >
            <v-icon>mdi-whatsapp</v-icon>
            
          </a>
        </v-btn>
        <v-btn id="btn" rounded="xl" variant="outlined" color="#754319" class="m-3 bg-white btnMove">
            <a
            :href="this.github"
            target="_blank"
            class="text-decoration-none text-black a-large "
          >
             <i class="my-iconA fab fa-git-alt"></i>
            github
          </a>
        </v-btn>
        </v-col>
      </div>
    </v-col>
  </v-row>
</template>

<script>
export default {
  props: {
    wa: String,
  },
  data() {
    return {
      whatsapp: "https://web.whatsapp.com/",
      github:"https://github.com/flaviovidalhuax",
      img:"https://i.imgur.com/goGA10y.jpg",
      vid:"https://i.imgur.com/j0qnFEP.mp4",
    };
  },
};
</script>


<style scope>
.btnMove:hover i{
  font-size:30px;
  transform: rotate(45deg);
  color:green;
}
</style>