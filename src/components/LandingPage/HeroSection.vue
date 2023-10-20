<template>
  <div>
    <v-row>
      <v-col cols="12" md="8" class="pr-md-10">
        <p class="text-h2 font-weight-bold white--text">
          Connect, Consult, and Care Remotely
        </p>
      </v-col>
      <v-col cols="12" md="4" class="ml-auto">
        <p class="body-1 white--text">
          Get high-quality service with quality telemedecine. Take control of
          your health and experience the benefits of telemedecine with our
          platform
        </p>
        <div class="d-flex flex-row align-center pr-md-10">
          <v-btn rounded block class="mr-2 py-7 px-16" color="#9CC4E1">Let's Talk!</v-btn>
          <v-btn fab><v-icon>mdi-play</v-icon></v-btn>
        </div>
      </v-col>
    </v-row>

    <div>
      <v-row class="px-16" id="images-container">
        <v-col cols="12" md="4">
          <v-img
            id="banner1"
            src="../../assets/hero banner 1.png"
            contain
          ></v-img>
        </v-col>
        <v-col cols="12" md="4">
          <v-img
            id="banner2"
            src="../../assets/hero banner 2.png"
            contain
          ></v-img>
        </v-col>
        <v-col cols="12" md="4">
          <v-img
            id="banner3"
            src="../../assets/hero banner 3.png"
            contain
          ></v-img>
        </v-col>
      </v-row>
      <v-img
        id="hero-banner-button"
        class="mx-auto"
        src="../../assets/hero banner button.png"
        contain
        max-width="200"
      ></v-img>

      <AboutUs id="about-us" />
    </div>
  </div>
</template>

<script>
import AboutUs from "./AboutUs.vue";

export default {
  name: "Heading",
  components: {
    AboutUs,
  },
};
</script>

<style scoped>
/* *{
      border: 1px solid gray;
  } */
#about-us {
  position: relative;
  z-index: 100;
  margin-top: -98px;
}

#banner1 {
  transform: rotate(-10deg);
  margin-top: 150px;
}

#banner3 {
  transform: rotate(10deg);
  margin-top: 150px;
}

#hero-banner-button {
  margin-top: -225px;
  position: relative;
  z-index: 200;
  }
</style>
