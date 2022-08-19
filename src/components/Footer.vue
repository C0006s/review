<template>
  <v-footer dark padless>
    <v-card flat tile class="black white--text py-12 px-5" width="100%">
        <v-row>
            <v-col cols="12" xs="12" sm="6" md="4" class="pa-16">
                <v-toolbar color="transparent" flat>
                    <v-badge color="black" dot>
                        <v-img src="cassete1.png" contain width="70"></v-img>
                    </v-badge>
                    <v-toolbar-title class="ml-4">
                        <span class="yellow--text"><strong>Cassette Store</strong></span>
                    </v-toolbar-title>
                </v-toolbar>
                <v-card-text class="pt-0">
                    <v-btn v-for="icon in icons" :key="icon" class="mx-1 white--text" icon fab outlined small>
                        <v-icon size="20px">
                            {{ icon }}
                        </v-icon>
                    </v-btn>
                </v-card-text>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="2">
                <v-card-text class="white--text pt-0">
                    <h3>About</h3>
                </v-card-text>
                <v-card-text class="grey--text">How It Work</v-card-text>
                <v-card-text class="grey--text">Refer A Friend</v-card-text>
                <v-card-text class="grey--text">Our Programs</v-card-text>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="2">
                <v-card-text class="white--text pt-0">
                    <h3>Delivery</h3>
                </v-card-text>
                <v-card-text class="grey--text">Cost On Delivery</v-card-text>
                <v-card-text class="grey--text">Payment Method</v-card-text>
                <v-card-text class="grey--text">Delivery Status</v-card-text>
                <v-card-text class="grey--text">Returns</v-card-text>
            </v-col>
            <v-col cols="12" xs="12" sm="6" md="2">
                <v-card-text class="white--text pt-0">
                    <h3>Contact</h3>
                </v-card-text>
                <v-card-text class="grey--text">08123456789</v-card-text>
                <v-card-text class="grey--text">bala@gmail.com</v-card-text>
                <v-card-text class="grey--text">Bandung</v-card-text>
            </v-col>
        </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default {
    data: () => ({
        icons: [
            "fab fa-google-plus-g",
            "fab fa-twitter",
            "fab fa-instagram",
            "fab fa-facebook",
        ],
    }),
}
</script>

<style>

</style>