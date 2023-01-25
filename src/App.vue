<template>
    <v-app id="inspire">
        <v-navigation-drawer
            v-model="drawer"
            app
        >
        <ul>
            <li>1</li>
            <li>2</li>
            <li>3</li>
        </ul>
        </v-navigation-drawer>


        <v-app-bar app>
            <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
            <v-toolbar-title>
                Application
            </v-toolbar-title>
        </v-app-bar>


        <v-main>
            <calendar />
        </v-main>
    </v-app>
</template>

<script>
import calendar from './components/calendar';

export default {
    name: 'App',
    
    components: {
        calendar,
    },
    data: () => ({ drawer: null }),
};
</script>
