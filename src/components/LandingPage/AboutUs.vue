<template>
  <div>
    <v-row class="container">
      <v-col cols="12" md="6" class="d-flex align-center">
        <p class="text-h5 font-weight-bold mx-auto mx-md-0 text-center text-md-left">About Us</p>
      </v-col>
      <v-col cols="12" md="6">
        <p class="text-h4 my-auto text-center text-md-left">
          We have a team of licensed healthcare professionals who are passionate
          about providing <span>high-quality</span> care through
          <span>iHealthMedz</span>
        </p>
      </v-col>

      <v-col>
        <v-row class="d-flex align-center">
          <v-col cols="12" md="6">
            <v-img
              src="../../assets/About Us 2.png"
              contain
              max-width="400"
              class="mx-auto"
            ></v-img>
          </v-col>

          <v-col cols="12" md="6">
            <div class="ml-md-4 mx-5">
              <div
                class="count mx-auto mx-md-0 mb-6 d-flex align-center justify-center"
              >
                <h3 class="pa-auto white--text">01</h3>
              </div>
              <p class="text-h4 mb-6 text-center text-md-left">
                Virtual Consultations
              </p>
              <p class="text-body-1 mb-6 text-center text-md-left">
                Patients can connect with healthcare providers for consultations
                from the comfort of their homes, without having to travel to an
                office or clinic.
              </p>

              <div
                class="d-flex align-center justify-space-between mb-10 mx-auto mx-md-0"
                id="buttons"
              >
                <v-img
                  src="../../assets/Chat button.png"
                  contain
                  class="mr-4"
                ></v-img>
                <v-img src="../../assets/Call button.png" contain></v-img>
              </div>

              <v-divider class="dividers mx-auto"></v-divider>
            </div>
          </v-col>
        </v-row>

        <v-row class="d-flex align-center">
          <v-col cols="12" md="6">
            <div class="d-flex justify-center">
              <v-card
                flat
                min-width="175"
                max-width="175"
                class="data1 pa-2 mr-4 d-flex flex-column justify-center"
              >
                <v-card-title class="mx-auto text-h2 font-weight-bold"
                  >325</v-card-title
                >
                <v-card-text class="text-center">
                  <p class="text-body-1">Doctor and Specialist</p>
                </v-card-text>
              </v-card>
              <v-card
                flat
                min-width="175"
                max-width="175"
                class="data2 pa-2 d-flex flex-column justify-center"
              >
                <v-card-title class="mx-auto text-h2 font-weight-bold"
                  >20k</v-card-title
                >
                <v-card-text class="text-center">
                  <p class="text-body-1 white--text">Patient in Case</p>
                </v-card-text>
              </v-card>
            </div>
          </v-col>

          <v-col cols="12" md="6">
            <div class="ml-md-4">
              <div
                class="count mx-auto mx-md-0 mb-6 d-flex align-center justify-center"
              >
                <h3 class="pa-auto white--text">02</h3>
              </div>
              <p class="text-h4 mb-6  text-center text-md-left">Remote patient monitor</p>
              <p class="text-body-1 mb-6 text-center text-md-left">
                Patients can use wearables or devices to collect and send health
                data to healthcare providers for monitoring.
              </p>

              <v-divider class="dividers mx-auto"></v-divider>
            </div>
          </v-col>
        </v-row>

        <v-row class="d-flex align-center">
          <v-col cols="12" md="6">
            <v-img
              src="../../assets/About Us 1.png"
              contain
              max-width="400"
              class="mx-auto"
            ></v-img>
          </v-col>

          <v-col cols="12" md="6">
            <div class="ml-md-4">
              <div
                class="count mx-auto mx-md-0 mb-6 d-flex align-center justify-center"
              >
                <h3 class="pa-auto white--text">03</h3>
              </div>
              <p class="text-h4 mb-6 text-center text-md-left">
                Mental health services such counseling sessions <br />
                <span>with licensed therapists or psychiatrists</span>
              </p>

              <div class="d-flex align-center">
                <v-card-title class="ml-auto text-h6 font-weight-bold"
                  >See More</v-card-title
                >
                <v-img
                  src="../../assets/button.png"
                  contain
                  max-width="50"
                ></v-img>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "AboutUs",
};
</script>

<style scoped>
/* *{
      border: 1px solid gray;
  } */
.container {
  background-color: white;
  /* padding-top: 200px; */
}

.count {
  width: 50px;
  height: 50px;
  border-radius: 50px;
  background-color: #0f152b;
}

span {
  color: #3e92b6;
}

#buttons {
  background-color: #0f152b;
  width: 180px;
  border-radius: 100px;
  padding: 10px;
}

.dividers {
  background-color: #000000;
}

.data1 {
  border: 2px solid #5a6282;
  border-radius: 50px;
  color: #0f152b;
}

.data2 {
  background-color: #0f152b;
  border-radius: 50px;
  color: white;
}
</style>
