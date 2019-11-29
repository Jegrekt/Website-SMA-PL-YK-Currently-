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
                   
                  </v-icon>
               </v-card-text>
               <v-card-text>
                  <v-flex class="text-sm-left">
                     <p >VISI SMA PANGUDI LUHUR YOGYAKARTA
                      Terbentuknya pribadi beriman, berbudi pekerti luhur, cerdas, terampil dan terbuka dalam menghadapi tantangan zaman.
                      MISI SMA PANGUDI LUHUR YOGYAKARTA
                      1. Mendampingi peserta didik menuju pribadi yang beriman.
                      2.Mendampingi peserta didik menuju pribadi yang berbudi pekerti luhur
                      3.Mendampingi peserta didik menuju pribadi yang cerdas
                      4.Mendampingi peserta didik menuju pribadi yang terampil
                      5.Mendampingi peserta didik menuju pribadi yang terbuka menghadapi tantangan zaman
                      Tujuan SMA PANGUDI LUHUR
                      1. Menghasilkan peserta didik yang beriman tanpa membedakan agama, ras, suku dan tingkat sosial.
                      2. Menghasilkan peserta didik yang menghidupi sikap kerja keras, tanggung jawab, setia, tangguh, jujur dan sederhana.
                      3. Menghasilkan peserta didik yang berpengetahuan dan dapat diterima di perguruan tinggi.
                      4. Menghasilkan peserta didik yang mampu menghargai dan melestarikan budaya lokal.
                      5. Menghasilkan peserta didik yang berbudaya dan berwawasan Ilmu Pengetahuan dan Teknologi.
                      Manfaat Bersekolah di SMA PANGUDI LUHUR YOGYAKARTA
                      1. Menghasilkan siswa yang Cerdas, Berbudi Pekerti Luhur
                      2. Menghasilkan siswa yang tangguh terhadap tantangan zaman
                      3. Membentuk kebribadian siswa yang takut dan bertakwa kepada Tuhan Yang Maha Esa
                      4. Membentuk karakter siswa agar dapat mengikuti perkembangan Zaman
                     </p>
                  </v-flex>
                   <h3>
                   </h3>
               </v-card-text>
            </v-card>
           </v-flex>
           <v-flex sm12 lg6 xl6>
              <v-card class="rounded" elevation="10">
                 <v-card-text class="text-xs-center">
                    <v-icon  color="primary" class="text-xs-center" size="100"></v-icon>
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
                     <v-icon size="200"></v-icon>
                  </v-flex>
                  <v-flex>
                     <v-btn
                     outline round large
                    :to="{path: '/'}"
                     >
                     home
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