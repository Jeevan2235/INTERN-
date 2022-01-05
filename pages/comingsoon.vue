<template>
  <div style="background-color: #f4f5fa">
    <v-row justify="center">
      <v-card width="50em" color="#f4f5fa" elevation="0">
        <p
          class="text-center mt-16"
          style="font-size: 1.5rem; color: rgba(94, 86, 105, 0.87)"
        >
          We are launching soon 🚀
        </p>
        <p class="text-center" style="color: rgba(94, 86, 105, 0.87)">
          Our website is opening soon. Please register to get notified when it's
          ready!
        </p>
        
        <v-row align="center" justify="center">
          <v-col col="12" md="5">
            <v-text-field
              outlined
              label="Enter your e-mail or username"
              hide-details="true"
            ></v-text-field>
          </v-col>
          <v-col cols="12" md="2">
            <v-btn height="3em" width="8em" color="#9155fd" class="white--text"
              >notify</v-btn
            >
          </v-col>
        </v-row>

        <v-img src="19.png" class="mt-10 ma-5"></v-img>
      </v-card>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>