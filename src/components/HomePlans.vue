<template>
    <v-container grid-list-lg>
        <v-layout row>
            <v-flex xs12 class="text-xs-center display-1 font-weight-black my-5">Available Meal Plans</v-flex>
        </v-layout>
        <v-layout row wrap>
            <v-flex xs12 sm12 md4 v-for="item in items" :key="item.id">
                <v-card>
                    <v-img :src="item.src" height="500px">
                        <v-container fill-height fluid>
                            <v-layout fill-height>
                                <v-flex xs12 align-end flexbox>
                                    <span class="headline white--text">{{ item.title }}</span>
                                </v-flex>
                            </v-layout>
                        </v-container>
                    </v-img>

                    <v-card-title primary-title>
                        <div>
                            <h3 class="headline mb-0">{{ item.subtitle}}</h3>
                            <div>{{ item.description }}
                            </div>
                        </div>
                    </v-card-title>
                </v-card>
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
                    subtitle:'Keto',
                    description:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam mauris felis, varius rutrum massa a, dignissim ornare dui. Cras eget velit eu dui tristique lobortis sit amet vel tellus.",
                    src: ('http://source.unsplash.com/hjCA3ecCXAQ'),
                },
                {
                    id: 2,
                    title:'PALEO',
                    subtitle:'Paleto',
                    description:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam mauris felis, varius rutrum massa a, dignissim ornare dui. Cras eget velit eu dui tristique lobortis sit amet vel tellus.",
                    src: ('http://source.unsplash.com/6S27S6pZ6o0'),
                },
                {
                    id: 3,
                    title:'VEGAN',
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
</style>