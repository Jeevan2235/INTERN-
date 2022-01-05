<template>
  <div>
    <v-row >
      <v-col cols="12" md="2" class="ma-8">
        <v-card elevation="0">
          <v-img src="14.png"></v-img>
        </v-card>
      </v-col>
      <v-col cols="12" md="4" class="mt-8">
        <v-row>
          <v-col>
            <v-btn class="mt-5 white--text" color="#9155fd"
              >Upload NeW Photo</v-btn
            >
          </v-col>
          <v-col>
            <v-btn class="mt-5" outlined color="#ff595d">Reset</v-btn>
          </v-col>
        </v-row>
        <p class="mt-5">Allowed JPG, GIF or PNG. Max size of 800K</p>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="mr-8 ml-8" cols="12" sm="12" md="5">
        <v-text-field outlined label="Username" value="johnDoe"></v-text-field>
        <v-text-field
          outlined
          label="E-mail"
          value="johnDoe@example.com"
        ></v-text-field>
        <v-select
          :links="link"
          outlined
          label="Status"
          value="Active"
        ></v-select>
      </v-col>
      <v-col class="mr-8 ml-8" cols="12" sm="12" md="5">
        <v-text-field outlined label="Name" value="john Doe"></v-text-field>
        <v-text-field outlined label="Role" value="Admin"></v-text-field>
        <v-text-field
          outlined
          label="Company"
          value="Google.inc"
        ></v-text-field>
      </v-col>
    </v-row>
    <v-card color="#fff6e1" elevation="0" class="ml-8 mr-8">
      <v-row>
        <v-col cols="12" md="1">
          <v-icon class="ml-10" color="#ffb400">mdi-alert-outline</v-icon>
        </v-col>
        <v-col cols="12" md="5">
          <p style="color: #ffb400">
            Your email is not confirmed. Please check your inbox.
          </p>
          <p style="color: #ffb400">Resend Confirmation</p>
        </v-col>
      </v-row>
    </v-card>
    <v-row class="ma-8">
      <v-btn class="mb-10 ma-3 white--text" color="#9155fd">
        save changes</v-btn
      >
      <v-btn class="mb-10 ma-3" outlined color="#adafb3">cancel</v-btn>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>