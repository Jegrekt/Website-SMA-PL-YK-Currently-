<template>
   <v-app>
      <v-content>
         <v-carousel
            height="700"
            >
         <v-carousel-item
         dark
         v-for="(item, i) in carousel"
         :key="i"
         :src="item.images"
         reverse-transition="fade"
         transition:="fade"
         ></v-carousel-item>
      </v-carousel>

      </v-content>
      
      <v-container grid-list-lg>
        <v-layout row wrap align-center justify-space-around>
         <v-flex xs12 sm12 lg6 xl6 color="blue">
            <v-card class="rounded" elevation="10">
               <v-card-text>
                  <v-icon class="text-xs-center" size="100" color="primary">
                   fa fa-
                  </v-icon>
               </v-card-text>
               <v-card-text>
                   <h3>Ini adalah Website SMA Pangudi Luhur Yogyakarta. Website ini dikelola oleh Team IT SMA Pangudi Luhur yang akan diupdate setiap harinya ketika terdapat event atau agenda baru yang diberikan oleh sekolah</h3>
               </v-card-text>
            </v-card>
           </v-flex>
           <v-flex sm12 lg6 xl6>
              <v-card class="rounded" elevation="10">
                 <v-card-text class="text-xs-center">
                    <v-icon  color="primary" class="text-xs-center" size="100">fa fa-</v-icon>
                 </v-card-text>
                 <v-card-text>
                    <h3>Founded at 7 November 2019</h3>
                    <h3>Managed by : Team IT SMA PL Yogyakarta</h3>
                 </v-card-text>
                 <v-card-text>
                 </v-card-text>
              </v-card>
           </v-flex>
        </v-layout>
      </v-container>
      <template>
      <v-container grid-list-lg>
         <v-layout>
            <v-flex>
               <v-card class="rounded1" elevation="5">
                  <v-card-text class="headline text-xs-center">
                     WEBSITE SMA PL YOGYAKARTA
                  </v-card-text>
                  <v-layout align-center justify-space-around>
                     <v-flex>
                     <v-icon size="200"> fa fa-</v-icon>
                  </v-flex>
                  <v-flex>
                     <v-btn
                     outline round large
                     :to="{path: '/contacts'}"
                     >
                     contacts
                  </v-btn>
                  </v-flex>
                  </v-layout>
               </v-card>
            </v-flex>
         </v-layout>
      </v-container>     
      </template>
      <footer-app></footer-app>
   </v-app>
</template>
<script>
export default {
   data:() => ({
      carousel:[
         {images: "/assets/Image1.jpg"},
         {images: "/assets/Image2.jpg"},
         
      ]
   }),
   methods: {
      // 
   }
}
</script>