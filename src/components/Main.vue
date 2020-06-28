<template>
    <div class="area">
        <v-container fluid style="height: 100vh;"
                     class="elevation-6">
            <v-container fluid fill-height grid-list-xl>
                <v-layout row wrap align-center>
                    <v-flex xs8 md5 text-xs-center style="text-align: right; z-index: 2;">
                        <h1 class="display-2 mb-2">Fullstack Web and Software Developer</h1>
                        <h2>
                            1 year web development experience
                            <em style="display:block;font-size:1rem;">- VueJS, ReactJS, Vuetify, Bootstrap, Bulma
                                <br/>
                                - Python, HTML, CSS, JavaScript, TypeScript, Java, Rust</em>
                        </h2>
                    </v-flex>
                    <v-flex xs12 md2 text-xs-center my-4 d-none d-sm-none d-md-flex style=" z-index: 2;">
                        <transition>
                            <v-avatar
                                    class="grey lighten-4"
                                    size="300"
                            >
                                <img src="https://avatars2.githubusercontent.com/u/47921345?s=460&u=db1f69067be410fc694754c159f81d100638c048&v=4"/>
                            </v-avatar>
                        </transition>
                    </v-flex>
                    <v-flex xs8 md3 text-xs-center class="d-none d-lg-none d-xl-inline"
                            style="text-align: left; z-index: 2;">
                        <h1 class="display-2 mb-3">More Information about me</h1>
                        <h3>
                            Age: 14<br/>
                            Gender: Male <br/>
                        </h3>
                    </v-flex>
                </v-layout>
            </v-container>
        </v-container>
        <ul class="circles">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
        <ul class="circles c-2">
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>
</template>
<script>
    export default {
        name: "Main"
    }
</script>
<style>
    .area {
        background: linear-gradient(to left, #7d81f3, #4e54c8);
        width: 100%;
        height: 100vh;
    }

    .circles {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        overflow: hidden;
    }

    .circles li {
        position: absolute;
        display: block;
        list-style: none;
        width: 20px;
        height: 20px;
        background: rgba(255, 255, 255, 0.3);
        animation: animate 15s linear infinite;
        bottom: 80vh;

    }

    .c-2 li {
        position: absolute;
        display: block;
        list-style: none;
        width: 20px;
        height: 20px;
        background: rgba(255, 255, 255, 0.3);
        animation: animate-2 15s linear infinite;
        top: -20vh;
    }

    .circles li:nth-child(1) {
        left: 25%;
        width: 80px;
        height: 80px;
        animation-delay: 0s;
    }


    .circles li:nth-child(2) {
        left: 10%;
        width: 20px;
        height: 20px;
        animation-delay: 2s;
        animation-duration: 12s;
    }

    .circles li:nth-child(3) {
        left: 70%;
        width: 20px;
        height: 20px;
        animation-delay: 4s;
    }

    .circles li:nth-child(4) {
        left: 40%;
        width: 60px;
        height: 60px;
        animation-delay: 0s;
        animation-duration: 18s;
    }

    .circles li:nth-child(5) {
        left: 65%;
        width: 20px;
        height: 20px;
        animation-delay: 0s;
    }

    .circles li:nth-child(6) {
        left: 75%;
        width: 110px;
        height: 110px;
        animation-delay: 3s;
    }

    .circles li:nth-child(7) {
        left: 35%;
        width: 150px;
        height: 150px;
        animation-delay: 7s;
    }

    .circles li:nth-child(8) {
        left: 50%;
        width: 25px;
        height: 25px;
        animation-delay: 15s;
        animation-duration: 45s;
    }

    .circles li:nth-child(9) {
        left: 20%;
        width: 15px;
        height: 15px;
        animation-delay: 2s;
        animation-duration: 35s;
    }

    .circles li:nth-child(10) {
        left: 85%;
        width: 150px;
        height: 150px;
        animation-delay: 0s;
        animation-duration: 11s;
    }

    .circles li:nth-child(11) {
        left: 75%;
        width: 110px;
        height: 110px;
        animation-delay: 3s;
    }

    .circles li:nth-child(12) {
        left: 75%;
        width: 110px;
        height: 110px;
        animation-delay: 3s;
    }

    @keyframes animate {

        0% {
            transform: translateY(0) rotate(0deg);
            opacity: 1;
            border-radius: 0;
        }

        100% {
            transform: translateY(-120vh) rotate(720deg);
            opacity: 0;
            border-radius: 100%;
        }

    }

    @keyframes animate-2 {

        0% {
            transform: translateY(0) rotate(0deg);
            opacity: 1;
            border-radius: 0;
        }

        100% {
            transform: translateY(120vh) rotate(720deg);
            opacity: 0;
            border-radius: 100%;
        }

    }
</style>