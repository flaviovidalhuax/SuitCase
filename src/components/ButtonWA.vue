<template>
  <div class="btn-wa" @mouseover="hover = true" @mouseout="hover = false">
    <a :href="whatsapp" target="_blank" class="text-decoration-none text-green d-flex justify-content-center align-items-center what">
      <v-icon size="x-large" class=" { 'd-none': !hover }">mdi-whatsapp</v-icon>
    </a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      whatsapp: "https://web.whatsapp.com/",
      hover: false,
    };
  },
};
</script>

<style scoped>
.btn-wa a {
  width: 70px;
  height: 70px;
}
.btn-wa {
  position: fixed;
  bottom: 10%;
  right: 0;
  background-color: #F3E5F5;
  color: white;
  border: 1px solid ;
  border-radius: 50% 0 0 50%;
  width: 70px;
  height: 70px;
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: width 0.2s;
}
.what {
  transform: rotate(45deg);
}

.btn-wa:hover {
  width: 140px;
  border-radius: 50px 0 0 50px;
 
}

.btn-wa a:hover {
  width: 140px;
  border-radius: 50px 0 0 50px;
  transform: rotate(-15deg);
}
</style>