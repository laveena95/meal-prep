<template>
    <v-container fluid fill-height class="home-hero" style="max-height: 100vh;" >
        <v-layout justify-center align-center column pa-5>
            <div class="display-4  white--text text-xs-center">HEALTHY MEALS</div>
            <div class="display-4 white--text text-xs-center mb-3">FOR YOUR TABLE</div>
            <v-btn fab class="mt-5 brown darken-4">
                <v-icon large color="white">mdi-chevron-down</v-icon>
            </v-btn>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'HomeHero'
};
</script>

<style scoped>
.home-hero {
    background: url('https://images.unsplash.com/photo-1455619452474-d2be8b1e70cd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=750&q=80');
    background-size: cover;
    width: 100%;
    height: 100%;
}
</style>