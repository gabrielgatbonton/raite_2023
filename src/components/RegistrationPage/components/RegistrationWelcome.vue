<template>
  <div>
    <v-container fluid>
      <v-row class="mx-3" justify="center">
        <v-col cols="auto" md="6" sm="12" align-self="center">
          <v-row>
            <v-col cols="12" lg="12" md="12" sm="6" xs="12">
              <div class="text-h2 font-weight-bold font mb-4">Welcome to</div>
            </v-col>
            <v-col cols="12" lg="12" md="12" sm="6" xs="12">
              <v-img
                width="500"
                contain
                alt="Logo Black "
                src="@/assets/Hackathon Assets/Logo Black.png"
              ></v-img>
            </v-col>
          </v-row>
        </v-col>
        <v-spacer></v-spacer>
        <v-col cols="auto" md="6" sm="12">
          <div class="container">
            <v-img
              width="425"
              contain
              alt="Registration Page 1"
              src="@/assets/Hackathon Assets/Registration page 1.png"
            ></v-img>
            <div :class="$vuetify.breakpoint.sm ? '' : 'centered'">
              Join our community and unlock a world of exciting possibilities.
              Registering is quick and easy. Get started now!
            </div>
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <div class="my-5 container">
            <v-row>
              <v-col cols="12">
                <v-img
                  class="mx-auto"
                  width="100%"
                  contain
                  alt="Registration Page 2"
                  src="@/assets/Hackathon Assets/Registration page 2.png"
                ></v-img>
              </v-col>
              <v-col
                :cols="
                  $vuetify.breakpoint.md
                    ? 6
                    : 12 || $vuetify.breakpoint.sm
                    ? 12
                    : ''
                "
              >
                <div
                  :class="
                    $vuetify.breakpoint.md || $vuetify.breakpoint.sm
                      ? ''
                      : 'top-left'
                  "
                >
                  <v-chip outlined color="black" class="px-8">
                    Our Team
                  </v-chip>
                  <div class="d-flex" style="margin-top: 20px">
                    <div class="my-2 text-h3 font-weight-bold">50+</div>
                    <div
                      style="display: block; width: 250px; margin-left: 20px"
                      class="text-subtitle-1 font-weight-bold compress"
                    >
                      Our team contains more than 50 qualified healthcare
                      professionals worldwide
                    </div>
                  </div>
                </div>
              </v-col>
              <v-col :cols="$vuetify.breakpoint.md ? 6 : 12">
                <div :class="$vuetify.breakpoint.md ? '' : 'bottom-right'">
                  <v-chip outlined color="black" class="px-8">
                    Why Register
                  </v-chip>
                  <v-container>
                    <v-row dense>
                      <v-col cols="auto">
                        <div class="border-radius my-auto">01</div>
                      </v-col>
                      <v-col cols="auto my-auto">
                        <div>Connect with healthcare professionals.</div>
                      </v-col>
                    </v-row>
                    <v-row dense>
                      <v-col cols="auto">
                        <div class="border-radius my-auto">02</div>
                      </v-col>
                      <v-col cols="auto my-auto">
                        <div>Schedule medical appointments online.</div>
                      </v-col>
                    </v-row>
                    <v-row dense>
                      <v-col cols="auto">
                        <div class="border-radius my-auto">03</div>
                      </v-col>
                      <v-col cols="auto my-auto">
                        <div>Access your health records securely.</div>
                      </v-col>
                    </v-row>
                    <v-row dense>
                      <v-col cols="auto">
                        <div class="border-radius my-auto">04</div>
                      </v-col>
                      <v-col cols="auto my-auto">
                        <div>Receive personalized health recommendations.</div>
                      </v-col>
                    </v-row>
                  </v-container>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <v-img
      width="100%"
      src="@/assets/Hackathon Assets/Slider 2.png"
      class=""
    ></v-img>
    <v-container fluid>
      <v-row no-gutters>
        <v-col cols="12" class="my-5">
          <div class="text-h1 text-center font-weight-bold">
            <span class="text-stroke text-h1 font-weight-bold">GET</span>
            STARTED
          </div>
        </v-col>
        <v-col cols="12"> </v-col>
      </v-row>
    </v-container>
    <v-card tile class="yellow">
      <div class="container">
        <v-img
          width="100%"
          class="mx-auto"
          style="
            width: 100%;
            object-fit: contain;
            margin-right: auto;
            margin-left: auto;
            display: block;
          "
          src="@/assets/Hackathon Assets/Contact without Blue Blur.png"
        ></v-img>
        <div
          class="text-h4 font-weight-bold"
          style="
            position: absolute;
            top: 120px;
            right: 180px;
            font-size: 18px;
            display: block;
            width: 280px;
            text-align: center;
          "
        >
          We take care about your health
        </div>
        <div style="position: absolute; top: 230px; right: 110px">
          <v-container>
            <v-row no-gutters>
              <v-col cols="12">
                <v-text-field
                  outlined
                  rounded
                  dense
                  style="width: 400px"
                  label="Last Name"
                  class="my-0 py-0"
                ></v-text-field>
                <v-text-field
                  outlined
                  rounded
                  dense
                  style="width: 400px"
                  label="First Name"
                  class="my-0 py-0"
                ></v-text-field>
                <v-text-field
                  outlined
                  rounded
                  dense
                  type="email"
                  style="width: 400px"
                  label="Email Address"
                  class="my-0 py-0"
                ></v-text-field>
                <v-text-field
                  outlined
                  rounded
                  dense
                  type="password"
                  style="width: 400px"
                  label="Password"
                  class="my-0 py-0"
                ></v-text-field>
              </v-col>
            </v-row>
          </v-container>
        </div>
        <div style="position: absolute; bottom: 240px; right: 135px">
          <v-checkbox
            class="my-checkbox my-0 py-0"
            label="By clicking 'Sign Up,'you agree to our [Terms of Service] and [Privacy Policy]."
          ></v-checkbox>
        </div>
        <div style="position: absolute; bottom: 200px; right: 240px">
          <v-btn rounded color="#9CC4E1" class="px-10 my-0 py-0">Sign Up</v-btn>
        </div>
        <div style="position: relative; bottom: 130px" class="container">
          <v-img src="@/assets/Hackathon Assets/Group 1.png"></v-img>
          <v-container>
            <v-row>
              <v-col cols="12">
                <div style="position: absolute; bottom: 250px; left: 100px">
                  <v-container class="mx-auto">
                    <v-row>
                      <v-col cols="12" md="6" sm="12">
                        <div
                          class="text-h2 font-weight-bold white--text text-center"
                          style="display: block; width: 550px"
                        >
                          Connect, Consult, and Care Remotely
                        </div>
                      </v-col>
                      <v-col cols="12" md="6" sm="12">
                        <div>
                          <div
                            class="text-subtitle-1 white--text text-center"
                            style="
                              display: block;
                              width: 280px;
                              line-height: 20px;
                              margin-left: 120px;
                            "
                          >
                            Get high-quality service with quality telemedecine.
                            Take control of your health and experience the
                            benefits of telemedecine with our platform
                          </div>
                          <div class="d-flex">
                            <div style="margin: 10px 0px 10px 120px">
                              <v-btn
                                rounded
                                color="#9CC4E1"
                                class="px-16 my-0 py-6"
                                >Let's Talk</v-btn
                              >
                            </div>
                            <div>
                              <v-img
                                style="margin: 10px 10px"
                                width="50"
                                contain
                                src="@/assets/Hackathon Assets/Play button.png"
                              ></v-img>
                            </div>
                          </div>
                        </div>
                      </v-col>
                    </v-row>
                  </v-container>
                </div>
              </v-col>
            </v-row>
          </v-container>
        </div>
      </div>
    </v-card>
  </div>
</template>

<script>
export default {};
</script>

<style>
.container {
  position: relative;
  width: 100%;
  text-align: left;
  color: black;
  font-size: 14px;
}
.centered {
  margin-left: 70px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.top-left {
  position: absolute;
  top: 8px;
  left: 16px;
}
.bottom-right {
  position: absolute;
  bottom: 0px;
  right: 40px;
}
.compress {
  margin-right: 100px;
}
.border-radius {
  border: 1px solid black;
  padding: 8px;
  padding-left: 11px;
  padding-right: 11px;
  border-radius: 20px;
}
.my-checkbox .v-label {
  font-size: 10px;
}
.text-stroke {
  color: black;
  -webkit-text-fill-color: white; /* Will override color (regardless of order) */
  -webkit-text-stroke-width: 3px;
  -webkit-text-stroke-color: black;
  font-size: 30px;
}
</style>
