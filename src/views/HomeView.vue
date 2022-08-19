<template>
  <v-app>
    <Navbar />
    <v-container fluid>
        <v-row>
          <v-col cols="12">
            <v-card class="mx-auto rounded-xl" flat>
              <v-img src="wall3.png" max-height="100%" max-width="100%" contain>
                <v-card-title class="top ml-10">
                  <h2 class="white--text title1">Order Your Music</h2> 
                </v-card-title>
                <v-card-title class="ml-10 mt-n8">
                  <h2 class="white--text title2">Bring Music Into Your Life !!</h2>
                </v-card-title>
                <v-card-text class="ml-10">
                  <h3 class="yellow--text">#Overseas Shipping Discount</h3>
                </v-card-text>
                <v-card-text class="ml-10">
                  <v-row>
                    <v-col cols="3">
                      <v-text-field label="Search your music" class="d-none d-sm-none d-md-flex"
                      filled solo prepend-inner-icon="mdi-magnify" flat rounded>
                      </v-text-field>
                    </v-col>
                    <v-col cols="2" class="marginleft">
                      <v-btn color="yellow" rounded dark x-large class="py-7 d-none d-smnone d-md-flex">search</v-btn>
                    </v-col>
                  </v-row>
                </v-card-text>
              </v-img>
            </v-card>
            <v-toolbar flat color="trasnparent">
              <v-toolbar-title class="text-h6">Category</v-toolbar-title>
              <v-spacer></v-spacer>
              <v-btn-toggle v-model="toggle_exclusive" group color="#F9BE00">
                <v-btn>
                  <v-icon>mdi-chevron-left</v-icon>
                </v-btn>
                <v-btn>
                  <v-icon>mdi-chevron-right</v-icon>
                </v-btn>
              </v-btn-toggle>
            </v-toolbar>
            <category/>
            <v-toolbar flat color="transparent" class="mt-5">
              <v-toolbar-title class="text-h6">Popular</v-toolbar-title>
              <v-spacer></v-spacer>
              <v-btn rounded color="yellow" dark class="px-8">See All</v-btn>
            </v-toolbar>
            <product />
            <v-card flat color="#fafafa" class="mt-8 py-5 px-16">
            <div style="
            position: absolute; margin-left: auto; margin-right: auto; left:0;
            right:0; text-align: center;">
            <h3>Services</h3>
            </div>
            <Service />
            </v-card>
            <v-toolbar flat colo="trasnparent" class="mt-8">
              <v-toolbar-title class="text-h6">
                Our Trusted Partner
              </v-toolbar-title>
            </v-toolbar>
            <Partner />
          </v-col>
        </v-row>
      </v-container>
      <Footer />
    </v-app>
  </template>

<script>
import Category from '../components/Category.vue'
  import Navbar from '../components/Navbar'
import Product from '../components/Product.vue'
import Service from '../components/Service.vue'
import Partner from '@/components/Partner.vue'
import Footer from '@/components/Footer.vue'

  export default {
    name: 'Home',
    data: () => ({
      toggle_exclusive: 1
    }),

    components: {
    Navbar,
    Category,
    Product,
    Service,
    Partner,
    Footer
},
  }

        Product</script>
<style>

.marginleft {
  margin-left: -90px;
}

.mtop {
  margin-top: 100px;
}

.mbottom {
  margin-bottom: 100px;
}

.v-card.borderme {
  border: 2px solid black !important;
}

.v-card.borderout {
  border: 1px solid #d5f0db !important;
}

.v-btn:not(.v-btn--round).v-size--default.add {
  min-width: 0px !important;
}

.theme--light.v-sheet--outlined.mobile {
  border: 2px solid black !important;
}

@media only screen and (max-width: 600px) {
  h2.title1 {
    
    font-size: 15px;  
  }
  h2.title2 {
    font-size: 15px;
  }
  .top {
    margin-top: 20px;
  }
}

@media only screen and (min-width: 600px){
  .top {
    margin-top: 20px;
  }
}

@media only screen and (min-width: 768px) {
  .top {
    margin-top: 120px;
  }
}
</style>
