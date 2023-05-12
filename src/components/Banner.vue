<template>
  <div
    id="banner-1"
    style="position: relative; height: 400px"
    class="text-white py-5 my-5"
  >
    <div
      style="
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-position: center;
        background-size: cover;
        filter: brightness(50%);
      "
      :style="backgroundImage"
    ></div>
    <div
      style="position: relative; z-index: 1; height: 400px"
      class="container py-lg-5 d-flex flex-column justify-content-center"
    >
      <h2 class="fw-bold w-50">
        Software Developer <br />
        Developer in page web
      </h2>
      <span class="line-under-text my-2"></span>
      <div class="w-lg-50">
        <p>
          I am developer web with experience in create page web, to learn more technologies is one my objective. Below you could to download my resume. 
        </p>
        <p> Phone number: 5521159387</p>
      </div>
      <div class="mx-xs-auto">
        <v-btn id="btn" rounded="xl" variant="outlined" color="#754319" class="m-3 bg-white btnMove">
            <a
              :href="this.whatsapp"
              target="_blank"
              class="text-decoration-none text-black "
            >
              <i class="fab fa-whatsapp"></i>
              Contac me in WHATSAPP
            </a>
        </v-btn>
        <v-btn class="bg-white btnMove" rounded="xl" variant="outlined" color="black"  href="/src/public/resumeMay23.pdf" download>
        <i class="fas fa-file-download"></i>
          Donwload resume
        </v-btn>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    wa: String,
  },
  data() {
    return {
      banner: "https://i.imgur.com/imU8jdD.jpg",
      whatsapp: "https://web.whatsapp.com/",
    };
  },
  computed: {
    backgroundImage() {
      return `background-image: url("${this.banner}")`;
    },
  },
};
</script>

<style scoped>
.line-under-text {
  width: 50%;
  height: 5px;
  display: block;
  background-color: #d6d3d0;
}
</style>