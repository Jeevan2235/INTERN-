<template>
  <div class="mt-10">
    <v-row class="" >
      <v-col   md="6" sm="12" class="ma-8">
        <v-text-field outlined label="Current Password"></v-text-field>
        <v-text-field outlined label="New Password"></v-text-field>
        <v-text-field outlined label="Confirm New Password"></v-text-field>
      </v-col>
     
      <v-col  md="4" >
        <v-img class="ml-16" src="15.png" height="16em" width="180px"></v-img>
      </v-col>
    </v-row>
    <v-divider></v-divider>
    <v-row class=" ma-8">
      <v-icon>mdi-key-outline</v-icon>
      <p class="mt-3 ma-3">Two-factor authentication</p>
    </v-row>
    <div class="text-center">
      <v-btn elevation="0">
          <v-icon color="#9155fd">mdi-lock-outline</v-icon>
      </v-btn>
      <p class="ma-3" style="font-weight:bold">Two factor authentication is not enabled yet.</p>
      <p>
        Two-factor authentication adds an additional layer of
        <br />
        security to your account by requiring more than just a <br />
        password to log in. Learn more.
      </p>

    </div>
      <v-row class="ma-8  ">
            <v-btn class="mb-10 ma-3 white--text" color="#9155fd"> save changes</v-btn>
            <v-btn class="mb-10 ma-3" outlined color="#adafb3">cancel</v-btn>
        </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>