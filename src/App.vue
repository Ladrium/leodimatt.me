<template>
    <v-app style="overflow: hidden;">
        <Navbar/>
        <Main/>
        <v-container>
            <v-container grid-list-xl style="margin-top: 2rem;">
                <v-layout wrap>
                    <v-flex
                            v-for="(project, i) in projects"
                            :key="i"
                            xs12
                            sm4
                            lg3
                            :data-oas="project.data">
                        <Project class="p-card" :name="project.name" :url="project.url"
                                 :description="project.description"
                                 :tags="project.tags"
                                 :image="project.image"
                                 :data="project.data"/>
                    </v-flex>
                </v-layout>
            </v-container>
        </v-container>
        <Footer/>
    </v-app>
</template>

<script>

    export default {
        name: "App",
        data: () => ({
            projects: [{
                name: "Xenus",
                url: "https://xenus.xyz",
                description: "Xenus is a multi-functional discord bot originally founded by Anonymous Guy",
                image: "https://cdn.discordapp.com/avatars/595290375401242634/a01bcd12db4d609cc6f8a18a338ad2a9.png?size=1024",
                tags: ["Discord Bot", "Web Dashboard", "JavaScript", "Discord.JS", "VueJS"],
                data: "zoom-out-right"
            }, {
                name: "Padrium",
                url: "https://github.com/Ladrium/Padrium",
                description: "Padrium is a discord bot based on adventure and business games",
                image: "https://media.discordapp.net/attachments/706969008460791880/726493505744142357/Padrium.png?width=702&height=702",
                tags: ["Discord Bot", "TypeScript", "Discord.JS"],
                data: "zoom-out-up"
            }, {
                name: "Statistic Tracker",
                url: "https://npmjs.com/package/statistic_tracker",
                description: "Statistic Tracker is a NPM module for tracking statistics in different games",
                image: "https://cdn.discordapp.com/attachments/706969008460791880/726501392067330090/unknown.png",
                tags: ["Module", "NPM", "TypeScript", "Tracking"],
                data: "zoom-out-down"

            },
                {
                    name: "Religion",
                    url: "https://religion.leodimatt.me",
                    description: "Is my religion.",
                    tags: ["Website", "Religion", "VueJS"],
                    data: "zoom-out-left"
                }]
        }),
        mounted() {
            /*eslint-disable */
            AOS.init();
        },
        components: {
            Project: () => import("./components/Project"),
            Main: () => import("./components/Main"),
            Navbar: () => import("./components/Navbar"),
            Footer: () => import("./components/Footer")
        }
    };
</script>
<style>
    @import url('https://fonts.googleapis.com/css?family=Exo:400,700');

    html {
        scroll-behavior: smooth;
    }

    body {
        overflow-x: hidden !important;
    }

    #app {
        height: 200vh;
        font-family: Exo, "sans-serif";
    }
</style>
