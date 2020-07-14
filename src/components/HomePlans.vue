<template>
    <v-container grid-list-lg>
        <v-layout row background-color: green>
            <v-flex xs12 class="text-xs-center text-center display-1 font-weight-black my-5" style="font-family:'Grenze Gotisch';">Available Meal Plans</v-flex>
        </v-layout>
        <v-layout row wrap>
            <v-flex xs12 sm12 md4 v-for="item in items" :key="item.id" cols="6" md="4">
                <v-hover v-slot:default="{ hover }">
                    <v-card
                    class="mx-auto"
                    color="grey lighten-4"
                    max-width="600"
                    >
                    <v-img
                        :aspect-ratio="16/9"
                        :src="item.src"
                    >
                        <v-expand-transition>
                        <div
                            v-if="hover"
                            class="d-flex transition-fast-in-fast-out yellow darken-2 v-card--reveal display-3 font-weight-black"
                            style="height: 100%;"
                        >
                            {{ item.price }}
                        </div>
                        </v-expand-transition>
                    </v-img>
                    <v-card-text
                        class="pt-6"
                        style="position: relative;"
                    >
                        <v-btn
                        absolute
                        color="orange"
                        class="white--text"
                        fab
                        large
                        right
                        top
                        >
                        <v-icon>mdi-cart</v-icon>
                        </v-btn>
                        <div class="font-weight-light grey--text title mb-2">For the perfect meal</div>
                        <h3 class="display-1 font-weight-light orange--text mb-2">{{ item.title }}</h3>
                        <div class="font-weight-light title mb-2">
                        {{ item.description }}
                        </div>
                    </v-card-text>
                    </v-card>
                </v-hover>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'HomePlans',
    data(){
        return {
             items: [
                {
                    id: 1,
                    title:'KETO',
                    price :'$14',
                    subtitle:'Keto',
                    description:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam mauris felis, varius rutrum massa a, dignissim ornare dui. Cras eget velit eu dui tristique lobortis sit amet vel tellus.",
                    src: ('http://source.unsplash.com/hjCA3ecCXAQ'),
                },
                {
                    id: 2,
                    title:'PALEO',
                    price :'$10',
                    subtitle:'Paleto',
                    description:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam mauris felis, varius rutrum massa a, dignissim ornare dui. Cras eget velit eu dui tristique lobortis sit amet vel tellus.",
                    src: ('http://source.unsplash.com/6S27S6pZ6o0'),
                },
                {
                    id: 3,
                    title:'VEGAN',
                    price :'$16',
                    subtitle:'Vegan',
                    description:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam mauris felis, varius rutrum massa a, dignissim ornare dui. Cras eget velit eu dui tristique lobortis sit amet vel tellus.",
                    src: ('http://source.unsplash.com/1SPu0KT-Ejg'),
                },
            ]
        }
    }
};
</script>

<style scoped>
    .v-card--reveal {
    align-items: center;
    bottom: 0;
    justify-content: center;
    opacity: .5;
    position: absolute;
    width: 100%;
    }
</style>