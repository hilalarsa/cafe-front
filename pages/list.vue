<template>
<section>
        <v-layout
          column
          wrap
          class="my-12"
          align-center
        >
          <v-flex xs12 sm4 class="my-4">
            <div class="text-center">
              <h2 class="headline">Cafe populer di Malang</h2>
              <span class="subheading">
                Cari cafe favoritmu disini!
              </span>
            </div>
          </v-flex>
          <v-flex xs12>
            <v-container grid-list-xl>
              <v-layout row wrap align-center>

                <v-flex 
                  v-for="(item, index) in listCafe"
                  v-bind:key="index"
                  xs12 md4
                  >
                  <v-card flat class="transparent">
                    <v-card-text class="text-center">
                      <!-- <v-icon x-large class="blue--text text--lighten-2">mdi-palette</v-icon> -->
                      <img :src="item.image" width="150"/>
                    </v-card-text>
                    <v-card-title primary-title class="layout justify-center">
                      <div class="headline text-center">{{ item.name }}</div>
                    </v-card-title>
                    <v-card-text>
                      {{ item.text }}  
                    </v-card-text>
                  </v-card>
                </v-flex>

              </v-layout>
            </v-container>
          </v-flex>
        </v-layout>
      </section>
</template>
<script>
const dummyCafe = [
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
    {
        id:"1",
        name:"Wakrop Brewok",
        text: "Menikmati kopi di tempat yang nyaman menjadi poin plus. Karena itulah di cabang barunya. Warkop Brewok mencoba menghadirkan suasana senyaman mungkin. Berada di Jalan Terusan Candi Mendut No 37, cabang kedua Warkop Brewok ini mengusung tema backyard.",
        image: "/warkop1.jpeg"
    },
]
export default {
  data(){
    return {
      listCafe: dummyCafe
    }
  }   
}
</script>