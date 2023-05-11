<template lang="">
 <v-card
    color="grey-lighten-4"
    flat
    height="100px"
    rounded="0"
  >
    <v-toolbar
      extended
      extension-height="50"
    >
      <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon> -->

      <v-toolbar-title class="font-weight-black text-gray">Skill</v-toolbar-title>



    <div class="col">
     <v-btn icon>
        <v-icon>mdi-bootstrap</v-icon>
      </v-btn>
      Bootrap
    </div>
    <div class="col">
      <v-btn class="color-red" icon>
        <v-icon class="color-red">mdi-react</v-icon>
      </v-btn>
      React
    </div>
    <div class="col">
      <v-btn icon>
        <v-icon class="color-red">mdi-vuetify</v-icon>
      </v-btn>
      Vuetify
    </div>
    <div class="col">
        <v-btn icon >
            <v-icon>mdi-tailwind</v-icon>
        </v-btn>
        Tailwind
    </div>
    <div class="col">
        <v-btn icon>
            <v-icon >mdi-vuejs</v-icon>
        </v-btn>
        Vue.js
    </div>
    <div class="col">
        <v-btn icon>
            <i class="my-iconA fab fa-node"></i>
        </v-btn>
        Node.js
    </div>
    <div class="col">
        <v-btn icon>
             <v-icon >mdi-laravel</v-icon>
        </v-btn>
        Laravel
    </div>
    <div class="col">
        <v-btn icon>
             <i class="my-iconA fab fa-github"></i>
        </v-btn>
        Github
    </div>
    <div class="col">
        <v-btn icon>
             <i class="my-iconA fab fa-git-alt"></i>
        </v-btn>
        GitSystem   
    </div>
    <div class="col border-1 m-2" >
        <v-btn icon >
           <i class="my-iconA fab fa-css3"></i>
        </v-btn>
        Css
    </div>
        
    </v-toolbar>
  </v-card>
</template>
<script>
export default {
    
}
</script>
<style scope>
    .my-iconA {
  font-size: 34px;
  color: black;
}
</style>