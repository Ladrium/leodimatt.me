<template>
  <v-card
    dark
    :href="url"
    class="p-card"
    :data-aos="data"
    data-aos-duration="5000"
  >
    <v-card-title>{{ name }}</v-card-title>
    <v-card-subtitle>{{ description }}</v-card-subtitle>
    <v-img :src="image" style="max-height: 300px;" v-if="image" />
    <v-card-text>
      <v-chip
        class="white--text"
        color="info"
        small
        style="margin: .1rem .2rem;"
        v-for="tag in tags"
        :key="tag"
      >
        {{ tag }}
      </v-chip>
      <h1 style="height: 1.8rem;" v-if="tags.length < 5" />
    </v-card-text>
  </v-card>
</template>
<script>
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  name: "Project",
  props: ["name", "url", "image", "description", "tags", "data"],
  created() {
    AOS.init();
  },
};
</script>
<style>
.p-card {
  background: #0369ff !important;
  transition: 0.5s !important;
}

.p-card:hover {
  transform: scale(1.05);
  background: #304ffe !important;
}

.p-card:hover .v-image {
  max-height: 100% !important;
}
</style>
