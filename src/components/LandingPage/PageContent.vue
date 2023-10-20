<template>
  <v-row>
    <v-col cols="12" md="6">
      <p class="text-h4 mb-6">
        Pre-Clinical Intake That’s <br /><span>As Easy As Sending A Text</span>
      </p>
    </v-col>
    <v-col cols="12" md="6">
      <div class="d-flex">
        <v-spacer></v-spacer>
        <v-btn color="#9CC4E1" elevation="0" rounded class="py-7 px-16"
          >Learn More</v-btn
        >
      </div>
    </v-col>

    <div class="grid-container">
      <v-img
        class="grid-item-1"
        src="../../assets/Steps 1.png"
        contain
        max-height="200"
      ></v-img>
      <v-img
        class="grid-item-2"
        src="../../assets/Steps 2.png"
        contain
        max-height="200"
      ></v-img>
      <v-img
        class="grid-item-3"
        src="../../assets/Steps 3.png"
        contain
        max-height="200"
      ></v-img>
      <v-img
        class="grid-item-4"
        src="../../assets/Steps 4.png"
        contain
        max-height="200"
      ></v-img>
      <v-img
        class="grid-item-5"
        src="../../assets/Steps 5.png"
        contain
        max-height="200"
      ></v-img>
    </div>
  </v-row>
</template>

<script>
export default {
  name: "PageContent",
};
</script>

<style scoped>
/* *{
      border: 1px solid gray;
  } */
span {
  color: #3e92b6;
}

.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  row-gap: 50px;
  column-gap: 50px;
}

.grid-item-1 {
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 1;
  grid-column-end: 2;
}
.grid-item-2 {
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 1;
  grid-column-end: 4;
}

.grid-item-3 {
  grid-row-start: 2;
  grid-row-end: 3;
  grid-column-start: 1;
  grid-column-end: 2;
}
.grid-item-4 {
  grid-row-start: 2;
  grid-row-end: 3;
  grid-column-start: 1;
  grid-column-end: 3;
  margin-left: 20px;
}

.grid-item-5 {
  grid-row-start: 2;
  grid-row-end: 3;
  grid-column-start: 1;
  grid-column-end: 4;
  margin-left: 140px;
}
</style>
