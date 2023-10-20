<template>
    <v-row>
      <v-col>
        <v-img src="../../assets/Logo.png" max-width="100"></v-img>
      </v-col>
      <v-col>
        <div class="d-flex align-center">
          <p class="text-caption white--text my-auto">Register for free</p>
          <v-btn rounded class="ml-4" color="#9CC4E1">Login</v-btn>
        </div>
      </v-col>
      <v-col>
        <div class="d-flex">
          <p class="text-caption white--text mr-4">
            Choose your preferred doctor and time to book an appointment or
            consultation
          </p>
          <v-btn rounded icon><v-img width="57" src="../../assets/chat notif white.png"></v-img></v-btn>
        </div>
      </v-col>
    </v-row>
  </template>
  
  <script>
  export default {
    name: "Hero",
  };
  </script>
  
  <style scoped>
  /* *{
      border: 1px solid gray;
  } */
  </style>
  