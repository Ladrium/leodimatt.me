<template>
  <footer>
    <a href="mailto:me@leodimatt.me"
      ><v-icon color="white" large>mdi-email</v-icon>
      <p class="d-none d-xs-none d-sm-block">me@leodimatt.me</p></a
    >
    <a href="https://www.instagram.com/leomagpizza/"
      ><v-icon color="white" large>mdi-instagram</v-icon>
      <p class="d-none d-xs-none d-sm-block">@LeoMagPizza</p></a
    >
    <a href="https://discord.gg/x8qnpNv"
      ><v-icon color="white" large>mdi-discord</v-icon>
      <p class="d-none d-xs-none d-sm-block">Ladrium#0001</p></a
    >
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>
<style scoped>
footer {
  padding: 0.5rem;
  font-family: Arial, Helvetica, sans-serif;
  width: 100%;
  text-align: center;
  background: #263238;
  position: fixed;
  bottom: 0;
}
footer > a {
  display: inline-block;
  margin-top: 0.5rem;
  width: 15%;
  text-decoration: none;
  color: white;
}

i {
  transition: 0.5s !important;
  background: #7289da;
  border: 10px solid #7289da;
  border-radius: 50%;
}
i:hover {
  color: #7289da !important;
  border-color: white;
  background: white;
}

@media screen and (max-width: 1000px) {
  footer > a {
    width: 20%;
  }
}

@media screen and (max-width: 650px) {
  footer > a {
    width: 33%;
  }
}

@media screen and (min-width: 1000px) {
  footer {
    position: absolute;
  }
}
</style>
