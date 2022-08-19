<template>
  <v-app-bar app color="white" flat>
    <v-badge color="white" dot>
        <v-img src="cassete1.png" contain width="80"></v-img>
    </v-badge>
    <v-toolbar-title class="ml-4">
        <span class="yellow--text"><strong>Cassete Store</strong></span>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-badge color="black" overlap content="2" class="mr-2 mt-1">
        <v-avatar color="#F9BE00" size="40">
            <v-icon x-small color="black">far fa-heart</v-icon>
        </v-avatar>
    </v-badge>
    <v-badge color="black" overlap content="3" class="mr-2 mt-1">
        <v-avatar color="#F9BE00" size="40">
            <v-icon x-small color="black">fa fa-shopping-cart</v-icon>
        </v-avatar>
    </v-badge>
    <span class="grey--text d-none d-sm-flex">Hallo, <strong>Reza Fauzan Dzikri</strong></span>
    <v-avatar size="30" class="ml-2">
        <v-img src="des2.jpg"></v-img>
    </v-avatar>
    <v-btn icon dark>
        <v-icon x-small color="#878a9a">fas fa-chevron-down</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {

}
</script>

<style>
.v-toolbar__title{
   font-size: 1rem !important; 
}
</style>