<template lang="">
    <div>
     
        <v-carousel
      v-model="model"
      
      cycle
      interval="4000"
      class="h-auto "
      hide-delimiter-background
      hide-delimiters
    >
    <h1 class="p-1 m-1">Nuestros productos</h1>
    <template v-slot:prev="{ props }">
      <v-btn
        class='text-brown rounded-circle'
        variant="elevated"
        color="#333333"
        @click="props.onClick"
        size="50"
      >	<h1>&#8249;</h1></v-btn>
    </template>
    <template v-slot:next="{ props }">
      <v-btn
      class='text-brown rounded-circle'
        variant="elevated"
        color="#333333"
        @click="props.onClick"
        size="50"
      ><h1>&#8250;</h1></v-btn>
    </template>
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        
      >
      <v-sheet 
      color="#333333"
      height="100%"
      weight="100%"
      class="d-flex justify-center align-center text-center"
      > 
      <v-card
                color="#0C0B0B"
                theme="dark"  
                >
                <v-card-text >
                    <v-row class="d-flex justify-center align-center">
                       <v-col cols="6">
                        <v-img
                        :src="item.src"
                        height='500'
                        weight='400'
                        >
                        </v-img>
                       </v-col>
                       <v-col cols="6">
                            <h3>{{item.title}}</h3>
                            <p>{{item.describe}}</p>
                            <section class="m-3">
                                <v-layout class="overflow-visible" style="height: 56px;">
                                  <v-bottom-navigation
                                    v-model="value"
                                    :bg-color="color"
                                    mode="shift"
                                  >
                                    <v-btn>
                                      <a :href="item.weight" class="textDecotarion" > 
                                      <v-icon>mdi-book</v-icon>
                                      <span class="text-white">Link web</span>
                                    </a>
                                    </v-btn>
                                    <v-btn>
                                    <a :href="item.price" class="textDecotarion" >
                                      <v-icon>mdi-image</v-icon>
                                      <span class="text-white">github</span>
                                    </a>
                                    </v-btn>
                                   
                                    <v-btn>
                                    <a :href="item.demo" class="textDecotarion" >
                                      <v-icon icon="mdi-arrow-up-bold-box-outline"></v-icon>
                                      <span class="text-white">swagger</span>
                                    </a>
                                    </v-btn>
                                    
                                  </v-bottom-navigation>
                                </v-layout>
                            </section>
                       </v-col>
                    </v-row>
                </v-card-text>
              </v-card>         
          
        
      </v-sheet>  
      </v-carousel-item>

      <v-radio-group
        inline
        v-model="selected"
        class="position-absolute bottom-0 end-50 pr-5"
        style="z-index: 1"
      >
        <v-radio value="0" color="#BB916D"></v-radio>
        <v-radio value="1" color="#BB916D"></v-radio>
        <v-radio value="2" color="#BB916D"></v-radio>
      </v-radio-group>
    </v-carousel>
    </div>
</template>
<script>
export default {
    data() {
    return {
      selected: 0,
      model: 0,
      model2: "0",
      whatsapp: "https://wa.me/c/5214421681339",
      items: [
        {
          src: "src/assets/imgBack/RedSocial.png",
          title: "Api RedSocial (Back-end) Node.js",
          describe: "This one example of red social, you can create a post comment and follow a user and make a like",
          diagram:"https://dbdiagram.io/d/639bd8bf99cb1f3b55a1bffc",
          price:"https://github.com/flaviovidalhuax/redSocialAPI-backendNode",
          
        },
       {
        src: "src/assets/imgBack/NetflixClone.png",
        title: "Api Netflix clone (Back-end) Node.js",
        describe: "In this Api you can post a movie and sort out a movies o serial.",
        diagram:"https://dbdiagram.io/d/63f80ba2296d97641d835db4",
        price:"https://github.com/flaviovidalhuax/netflix-backEdn-node",
       },
       {
        src:"src/assets/imgBack/Chat.png",
        title: "Skeleton for backend-node.js",
        describe: "This Api is Back end of a chat like whatsapp, you can a create conversation and create a red of users and talk with friends",
        diagram:"https://dbdiagram.io/d/63e5c3c1296d97641d7fe093",
        price:"https://github.com/flaviovidalhuax/chat-test4node",
       },
       {
        src:"src/assets/imgBack/squeleton.png",
        title:"Skeleton for init your new project",
        describe: "This is my skeleton for reducing work when you init a new project, it is base the code in the backend and deploy  in Render.",
        diagram:" https://esqueleton-email.onrender.com",
        price:"https://github.com/flaviovidalhuax/squeton-email",
        demo:"https://esqueleton-email.onrender.com/api/v1/docs/",
       } 

      ],
    };
  },
  watch: {
    model(newVal, oldVal) {
      this.model2 = newVal;
      this.selected = newVal.toString();
    },
    selected(newVal, oldVal) {
      this.model = parseInt(newVal);
    },
  },
  computed: {
      color () {
        switch (this.value) {
          case 0: return 'indigo'
          case 1: return 'teal'
          case 2: return 'brown'
          case 3: return 'indigo'
          default: return 'blue-grey'
        }
      },
}
};   

</script>
<style lang="">
    
</style>