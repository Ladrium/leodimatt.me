<template>
  <v-app-bar
    fixed
    id="nav"
    style="background: transparent; transition: .5s; z-index: 7;"
    elevate-on-scroll
  >
    <v-spacer />
    <v-toolbar-title>
      Leonardo Di Matteo
    </v-toolbar-title>
    <v-spacer />
  </v-app-bar>
</template>
<script>
export default {
  name: "Navbar",
  mounted() {
    window.addEventListener("scroll", () => {
      const navbar = document.getElementById("nav");
      if (window.pageYOffset > 5) {
        navbar.style.background = "#263238";
        navbar.classList.add("theme--dark");
      } else {
        navbar.classList.remove("dark");
        navbar.style.background = "rgb(0, 0, 0, 0)";
      }
    });
  },
};
</script>
