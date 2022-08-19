<template>
  <v-row class="mt-10 mb-5">
    <v-col cols="12" xs="12" sm="6" md="4" v-for="(service, i) in services" :key="i">
        <v-card class="elevation-1 mx-auto" width="300">
            <v-list subheader two-line>
                <v-list-item>
                    <v-list-item-avatar>
                        <v-img :src="service.img"></v-img>
                    </v-list-item-avatar>
                    <v-list-item-content>
                        <v-list-item-title>{{ service.title }}</v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
            </v-list>
            <v-card-text>
                <div class="mt-n7">
                    <v-rating v-model="rating" color="yellow darken-1" background-color="grey darken-1"
                    empty-icon="$ratingFull" half-increments hover medium></v-rating>
                </div>
                {{ service.bio }}
            </v-card-text>
        </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
    data: () => ({

   
    rating: 4.5,
    services: [{
        img: "shield.png",
        title: "Trusted",
        bio: "Its Officialy Store"

    },{
        img: "cruise.png",
        title: "Shipping",
        bio: "All Around World"
    },{
        img: "guarantee.png",
        title: "Guaranteed",
        bio: "Money Back If Item Is Damaged"
    },]
 })
}
</script>

<style>

</style>