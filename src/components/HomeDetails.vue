<template>
    <v-container >
        <v-layout>
            <v-container>
                <div class="about">
                    <v-flex >
                        <h5>Delicious</h5>
                        <h2>PREMIUM</h2>
                        <h2>FOOD HOME</h2>
                    <v-flex>
                        <p class="subheading mt-3" max-width="300px">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras pulvinar risus quis mauris interdum, in euismod nibh pretium. Etiam pulvinar tincidunt dapibus. Quisque sollicitudin, mauris a consequat consectetur, turpis nisl sollicitudin enim, id consectetur neque neque nec metus.</p>
                        <v-img src="https://cdn.theforkmanager.com/static/styles/blog_article_header_image/public/wp-blog/5-el-tenedor-gestion-restaurantes-contratar-al-mejor-chef.jpg?itok=hDZiX5AS" height="400px" max-width="300px"></v-img>
                    </v-flex>
                    </v-flex>
                    <v-container>
                       
                    </v-container>
                </div>
            </v-container>
            <v-flex>
                <v-img src="http://source.unsplash.com/hjCA3ecCXAQ" max-height="900px" max-width="500px" align="right"></v-img>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'HomeDetails',
    data(){
        return {
        }
    }
};
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Arvo&display=swap');

.about{
    width: 400px;
    height: 600px;
    margin-left: 100px;
}
.about h5{
    font-family: 'Pacifico', cursive;
    font-size: 30px;
    color: red;
    
}
.about h2{
    font-family: 'Arvo', serif;
    font-size: 50px;
}
</style>