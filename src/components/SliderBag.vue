<template>
    <div id="carouselExampleCaptionsB" class="carousel slide colorSlider py-5 my-5">
    <div class="carousel-indicators ">
        <button type="button" data-bs-target="#carouselExampleCaptionsB" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
        <button type="button" data-bs-target="#carouselExampleCaptionsB" data-bs-slide-to="1" aria-label="Slide 2"></button>
        <button type="button" data-bs-target="#carouselExampleCaptionsB" data-bs-slide-to="2" aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner m-4">
      <div class="carousel-item active">
        <div class="row">
          <section class="col">
            <div class="card mb-3 bg-black rounded-3" style="max-width: 540px">
              <div class="row g-0">
                <div class="col-md-4">
                  <img
                    src="https://w0.peakpx.com/wallpaper/998/140/HD-wallpaper-pikachu-pokemon.jpg"
                    class="img-fluid rounded-start h-100 w-100"
                    alt="pikachu"
                  />
                </div>
                <div class="col-md-8">
                  <div class="card-body">
                    <h5 class="card-title font-weight-bold">Poke Api Rect.js</h5>
                    <p class="card-text  font-weight-medium">                                        
                      This is a api use React.js Css for style use Route, Redux, Hooks like (useState, useEffect). You Can find one pokemon with the name or power.
                    </p>
                    <section>
                      <v-layout class="overflow-visible" style="height: 56px;">
                      <v-bottom-navigation
                        v-model="value"
                        :bg-color="color"
                        mode="shift"
                      >
                        <v-btn>
                          <a :href="enlacePkeWeb" class="textDecotarion" > 
                          <v-icon>mdi-book</v-icon>

                          <span>Link web</span>
                        </a>
                        </v-btn>
                        <v-btn>
                        <a :href="enlacePke" class="textDecotarion" >
                         <i class="my-iconA fab fa-github"></i>
                          <span>github</span>
                        </a>
                        </v-btn>
                      </v-bottom-navigation>
                    </v-layout>
                    </section>
                  </div>
                </div>
              </div>
            </div>
          </section>
          <section class="col">
            <div class="card mb-3 bg-black rounded-3" style="max-width: 540px">
              <div class="row g-0">
                <div class="col-md-4">
                  <img
                    src="https://www.lluviadigital.com/wp-content/uploads/2020/02/e-commerce-que-es-Lluvia-Digital.jpg"
                    class="img-fluid rounded-start h-100 w-100"
                    alt="eccommer"
                  />
                </div>
                <div class="col-md-8">
                  <div class="card-body">
                    <h5 class="card-title font-weight-bold">Ecommerce Api React</h5>
                    <p class="card-text  font-weight-medium">                                        
                      This is a api use React.js Css for style use Route, Redux, axios, Hooks like (useState, useEffect, hoohform). You Can find a product for price and you can add card and buy it.
                    </p>
                    <section>
                      <v-layout class="overflow-visible" style="height: 56px;">
                      <v-bottom-navigation
                        v-model="value"
                        :bg-color="color"
                        mode="shift"
                      >
                        <v-btn>
                          <a :href="enlaceEcomer" class="textDecotarion" > 
                          <v-icon>mdi-book</v-icon>
                          <span>Link web</span>
                        </a>
                        </v-btn>
                        <v-btn>
                        <a :href="enlaceEcmGit" class="textDecotarion" >
                          <i class="my-iconA fab fa-github"></i>
                          <span>github</span>
                        </a>
                        </v-btn>
                      </v-bottom-navigation>
                    </v-layout>
                    </section>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>
        <!-- rick -->
        <div class="row">
          <section class="col">
            <div class="card mb-3 bg-black rounded-3" style="max-width: 540px">
              <div class="row g-0">
                <div class="col-md-4">
                  <img
                    src="https://es.web.img3.acsta.net/pictures/18/10/31/17/34/2348073.jpg"
                    class="img-fluid rounded-start h-100 w-100"
                    alt="pikachu"
                  />
                </div>
                <div class="col-md-8">
                  <div class="card-body">
                    <h5 class="card-title font-weight-bold">Rick and Morthy React</h5>
                    <p class="card-text  font-weight-medium">                                        
                      This is a api use React.js Css for style, axios, Hooks like (useState, useEffect). You Can find a for id number your favorite animate.
                    </p>
                    <section>
                      <v-layout class="overflow-visible" style="height: 56px;">
                      <v-bottom-navigation
                        v-model="value"
                        :bg-color="color"
                        mode="shift"
                      >
                        <v-btn>
                          <a :href="enlaceRickWeb" class="textDecotarion" > 
                          <v-icon>mdi-book</v-icon>
                          <span>Link web</span>
                        </a>
                        </v-btn>
                        <v-btn>
                        <a :href="enlaceRickGit" class="textDecotarion" >
                           <i class="my-iconA fab fa-github"></i>
                          <span>github</span>
                        </a>
                        </v-btn>
                      </v-bottom-navigation>
                    </v-layout>
                    </section>
                  </div>
                </div>
              </div>
            </div>
          </section>
          <!-- weather -->
          <section class="col">
            <div class="card mb-3 bg-black rounded-3" style="max-width: 540px">
              <div class="row g-0">
                <div class="col-md-4">
                  <img
                    src="https://scied.ucar.edu/sites/default/files/media/images/weather_0.jpg"
                    class="img-fluid rounded-start h-100 w-100"
                    alt="pikachu"
                  />
                </div>
                <div class="col-md-8">
                  <div class="card-body">
                    <h5 class="card-title font-weight-bold">Weather Api React</h5>
                    <p class="card-text  font-weight-medium">                                        
                      This is a api use React.js Css for style, axios, Hooks like (useState, useEffect). In this Api give the weather in your position of your gps.
                    </p>
                    <section>
                      <v-layout class="overflow-visible" style="height: 56px;">
                      <v-bottom-navigation
                        v-model="value"
                        :bg-color="color"
                        mode="shift"
                      >
                        <v-btn>
                          <a :href="enlaseWeatherWeb" class="textDecotarion" > 
                          <v-icon>mdi-book</v-icon>
                          <span>Link web</span>
                        </a>
                        </v-btn>
                        <v-btn>
                        <a :href="enlaseWeatherGit" class="textDecotarion" >
                           <i class="my-iconA fab fa-github"></i>
                          <span>github</span>
                        </a>
                        </v-btn>
                      </v-bottom-navigation>
                    </v-layout>
                    </section>
                  </div>
                </div>
              </div>
            </div>
          </section>
        </div>

            <!-- node -->
        </div>
        <div class="carousel-item  " >
            <div class="row">
          <section class="col ">
            <div class="card mb-3 bg-black rounded-3" style="max-width: 540px">
              <div class="row g-0">
                
                <div class="col-md-12">
                  <div class="card-body">
                    <h5 class="card-title font-weight-bold">Post your event Next.js</h5>
                    <p class="card-text  font-weight-medium">                                        
                      In this project work with the framework <span class="font-weight-bold">Next.js</span> and style use tailwind. In this Api work in team of 2 person the porpouse was use git.
                      We use SweetAlert and useSWRConfig hookfor, a library to use Swiper as a ReactJs component. 
                      You can create a user and post a event if a event like you therefore you can a vote.
                    </p>
                    <section>
                      <v-layout class="overflow-visible" style="height: 56px;">
                      <v-bottom-navigation
                        v-model="value"
                        :bg-color="color"
                        mode="shift"
                      >
                        <v-btn>
                          <a :href="enlaceNextWeb" class="textDecotarion" > 
                          <v-icon>mdi-book</v-icon>
                          <span>Link web</span>
                        </a>
                        </v-btn>
                        <v-btn>
                        <a :href="enlaceNextGit" class="textDecotarion" >
                          <i class="my-iconA fab fa-github"></i>
                          <span>github</span>
                        </a>
                        </v-btn>
                      </v-bottom-navigation>
                    </v-layout>
                    </section>
                  </div>
                </div>
              </div>
              <div class="col-md-10">
                  <img
                    src="/src/assets/img/next0.png"
                    class="img-fluid rounded-start h-100 w-100"
                    alt="node"
                  />
                </div>
            </div>
          </section>
          <section class="col">
             <div class="card-body"> 
                <div class="card mb-3 bg-black rounded-3" style="max-width: 540px">
                  <div class="row g-0">
                    <div class="col-md-5 ">
                      <img
                        src="/src/assets/img/next1.png"
                        class="img-fluid rounded-start h-100 w-100"
                        alt="next"
                      />
                    </div>
                    <div class="col-md-10">
                      <img
                        src="/src/assets/img/next2.png"
                        class="img-fluid rounded-start h-100 w-100"
                        alt="next"
                      />
                    </div>
                  </div>
                </div>
            </div>
              </section>
            </div>
            <!-- as -->
            
            
        </div>
   
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptionsB" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptionsB" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
    </button>
</div>
</template>
<script>
export default {
  data() {  
    return {
      enlacePkeGit: 'https://github.com/flaviovidalhuax/lastpokeapi',
      enlacePkeWeb: 'https://effervescent-faloodeh-042c84.netlify.app/',
      enlaceEcomer:'https://chipper-arithmetic-6802f2.netlify.app/',
      enlaceEcmGit:'https://github.com/flaviovidalhuax/EcommerReact18',
      enlaceRickGit:'https://github.com/flaviovidalhuax/rickandmorty',
      enlaceRickWeb:'https://brilliant-puffpuff-1bcead.netlify.app/',
      enlaseWeatherGit:'https://github.com/flaviovidalhuax/weather',
      enlaseWeatherWeb:'https://musical-centaur-c8bd4a.netlify.app/',
      enlaceNextGit:'https://github.com/flaviovidalhuax/NextEventosCity',
      enlaceNextWeb:'https://dashing-axolotl-47ab54.netlify.app/',
      value: 1,
      mage0:'/Commerce.png',
      mage1:'/rick.png',
      mage1:'/rallo.jpg',
      mage2:'/next2.png',
      mage2:'/next2.png',

    }
  },
  computed: {
      color () {
        switch (this.value) {
          case 0: return 'blue-grey'
          case 1: return 'teal'
          case 2: return 'brown'
          case 3: return 'indigo'
          default: return 'blue-grey'
        }
      },
}
}
</script>
<style scoped >
  .colorSlider{
    background:#0C0B0B;
  }
  .colorImage{
    background:#747474;
  }
  .textDecotarion {
    color:#ffff;
  text-decoration: none;
}
</style>