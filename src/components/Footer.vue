<template>
 <footer>
    <a href="mailto:me@leodimatt.me"><v-icon color="primary" large>mdi-email</v-icon><p class="d-none d-sm-none d-md-flex">me@leodimatt.me</p></a>
    <a href="https://www.instagram.com/leomagpizza/"><v-icon color="primary" large>mdi-instagram</v-icon><p class="d-none d-sm-none d-md-flex">@LeoMagPizza</p></a>
    <a href="https://discord.gg/x8qnpNv"><v-icon color="primary" large>mdi-discord</v-icon><p class="d-none d-sm-none d-md-flex">Ladrium#0001</p></a>
  </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>
<style scoped>
    footer {
        padding: .5rem;
        font-family: Arial, Helvetica, sans-serif;
        width: 100%;
        background: #263238;
        position: fixed;
        bottom: 0;
    }
    footer > a {
        margin-left: 20%;
        text-decoration: none;
        color: white;
        float: left;
    }

    i {
        transition: .5s !important;
    }
    i:hover {
        color: #00E5FF !important;    
    }
    @media screen and (max-width: 500px) {
        footer > a {
            margin-left: 15%;
        }
    }

    @media screen and (min-width: 1000px) {
        footer {
            position: absolute;
        }

    }
</style>