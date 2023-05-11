<template>
  <v-carousel
    v-model="model"
    class="position-relative vh-85 mb-5"
    cycle
    interval="3000"
    hide-delimiter-background
    hide-delimiters
    color="#BB916D"
  >
    <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src" cover>
      <div
        style="height: 100%"
        class="d-flex justify-content-center flex-column text-white container align-items-xs-center align-items-lg-start"
      >
        <h2 class="fw-bold w-50 font-weight-black">{{ item.title }}</h2>
        <span class="line-under-text my-2"></span>
        <div class="w-50">
          <p class="text-gray font-weight-black">{{ item.p }}</p>
          <v-btn id="btn" rounded="xl" variant="outlined" color="#754319" class="bg-white">
            <a
              :href="this.wa"
              target="_blank"
              class="text-decoration-none text-black a-large"
            >
              <v-icon>mdi-whatsapp</v-icon>
              contact me
            </a>

            <a
              :href="this.wa"
              target="_blank"
              class="text-decoration-none text-white a-small"
            >
              <v-icon>mdi-whatsapp</v-icon>
              contact me <br />
              WHATSAPP
            </a>
          </v-btn>
        </div>
      </div>
    </v-carousel-item>

    <v-radio-group
      inline
      v-model="selected"
      class="position-absolute bottom-0 end-0 pr-5"
      style="z-index: 1"
    >
      <v-radio value="0" color="#BB916D"></v-radio>
      <v-radio value="1" color="#BB916D"></v-radio>
      <v-radio value="2" color="#BB916D"></v-radio>
    </v-radio-group>
  </v-carousel>
</template>
<script >
export default {
  props: {
    wa: String,
  },
  data() {
    return {
      selected: 0,
      model: 0,
      whatsapp: "https://wa.me/c/5214421681339",
      items: [
        {
          src: "/desarrolloWeb.jpg",
          title: "Hello, I am Full-stack ",
          p: "I know the technologies in javascript in Front-end and Back-end ",
        },
        {
          src: "/lap.jpg",
          title: "Hello, I am Front Developer",
          p: "In front-end I work with React.js, Node.js, Vue.js; therefor I use CSS, HTML, bootstrap, ReactBostrap, Vuetify, Tailwind.    ",
          button: "CONTACTANOS",
        },
        {
          src: "/mac2.webp",
          title: "Hello, I am back end ",
          p: "In back-end I work with Node.js and Laravel 8",
        },
      ],
    };
  },
  watch: {
    model(newVal, oldVal) {
      this.selected = newVal.toString();
    },
    selected(newVal, oldVal) {
      this.model = parseInt(newVal);
    },
  },
};
</script>

<style scoped>
.line-under-text {
  width: 50%;
  height: 5px;
  display: block;
  background-color: #bb916d;
}
</style>