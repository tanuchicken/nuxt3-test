<template>
    <v-app>
        <v-app-bar dence color="blue">
            <v-app-bar-nav-icon
            @click="drawer=!drawer"></v-app-bar-nav-icon>
            <v-toolbar-title>this is header</v-toolbar-title>
        </v-app-bar>
        <v-navigation-drawer v-model="drawer" fixed>

        </v-navigation-drawer>

        <div>
            <nuxtPage />
        </div>
    </v-app>
</template>

<script>
export default {
    setup() {
        let drawer = ref(true)

        return {
            drawer
        }
    }
}
</script>