<template>
    <span>
        <v-toolbar app color="brown darken-4" dark>
            <div class="hidden-sm-and-up">
                <v-menu offset-y>
                    <template v-slot:activator="{ on }">
                        <v-app-bar-nav-icon
                            v-on="on"
                        ></v-app-bar-nav-icon>
                    </template>
                    <v-list class="brown lighten-2" dark>
                         <v-list-item>
                            <v-list-item-title>
                                Menu
                            </v-list-item-title>
                        </v-list-item>
                        <v-divider></v-divider>
                        <v-list-item>
                            <v-list-item-title>
                                About
                            </v-list-item-title>
                        </v-list-item>
                        <v-divider></v-divider>
                        <v-list-item>
                            <v-list-item-title>
                                SIGN IN
                            </v-list-item-title>
                        </v-list-item>
                        <v-divider></v-divider>
                        <v-list-item>
                            <v-list-item-title>
                                JOIN
                            </v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-menu>
            </div>
            <v-spacer class="hidden-md-and-up"> </v-spacer>
                <router-link to="/">
                    <v-toolbar-title style="color: white;">{{ appTitle }}</v-toolbar-title>
                </router-link>
                <v-btn flat class="hidden-sm-and-down" to="/menu">Menu</v-btn>
                <v-spacer class="hidden-sm-and-down"></v-spacer>
                <v-btn flat class="hidden-sm-and-down" to="/about">About</v-btn>
                <v-btn flat class="hidden-sm-and-down" to="/signin">SIGN IN</v-btn>
                <v-btn color="brown lighten-3" class="hidden-sm-and-down" to="/join">JOIN</v-btn>
        </v-toolbar>
    </span>
</template>

<script>
export default {
    name: 'AppNavigation',
    data() {
        return {
            appTitle: 'Meal Prep',
        };
    }
};
</script>

<style>
    a {
    color: white;
    text-decoration: none;
}
</style>
