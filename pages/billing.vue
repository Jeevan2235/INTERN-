<template>
  <v-row justify="center">
    <v-card class="mt-16" width="72em">
    <v-card elevation="4" tile>
      <v-row>
        <v-btn height="3em" class="ma-2" tile color="white" elevation="0">
          <v-icon class="ma-3">mdi-account-outline</v-icon>
          <p class="mt-4">Account</p>
        </v-btn>
        <v-btn height="3em" class="ma-2" tile color="white" elevation="0">
          <v-icon class="ma-3">mdi-account-outline</v-icon>
          <p class="mt-4">Security</p>
        </v-btn>
        <v-btn height="3em" class="ma-2" tile color="white" elevation="0">
          <v-icon class="ma-3">mdi-account-outline</v-icon>
          <p class="mt-4">Info</p>
        </v-btn>
        <v-btn height="3em" class="ma-2" tile color="white" elevation="0">
          <v-icon class="ma-3">mdi-account-outline</v-icon>
          <p class="mt-4">Billing</p>
        </v-btn>
        <v-btn height="3em" class="ma-2" tile color="white" elevation="0">
          <v-icon class="ma-3">mdi-account-outline</v-icon>
          <p class="mt-4">Notifications</p>
        </v-btn>
      </v-row>
    </v-card>
    <v-row class="ma-8">
      <v-col cols="12" md="8">
        <p>Payment Method</p>
        <v-radio-group v-model="row" row>
          <v-radio
            color="#9155fd"
            label="Credit/Debit/ATM Card"
            value="Male"
          ></v-radio>
          <v-radio color="#9155fd" label="COD/Cheque" value="Female"></v-radio>
        </v-radio-group>
        <v-text-field label="Name" value="john Doe" outlined></v-text-field>
        <v-text-field
          label="Card Number"
          value="13563 21565 48789"
          outlined
        ></v-text-field>
        <v-row class="ma-1">
          <v-text-field
            label="Expiry Date"
            value="0524"
            outlined
          ></v-text-field>
          <v-text-field
            v-model="password"
            :type="show1 ? 'text' : 'password'"
            label="CVV Code"
            class="ml-3"
            outlined
            @click:append="show1 = !show1"
          ></v-text-field>
        </v-row>
       
      </v-col>
      <v-col cols="12" md="4">
        <v-card outlined>
          <v-row class="ma-4">
            <v-checkbox color="#9155fd"></v-checkbox>
            <p class="mt-5">Your Current Plan</p>
          </v-row>
          <v-chip class="ml-4" style="color:#9155fd" small>Basic Plan</v-chip>
          <v-row class="ma-4">
              <v-icon>mdi-account-outline</v-icon>
              <p class="ma-2">5 Users</p>
          </v-row>
            <v-row class="ma-4">
              <v-icon>mdi-account-outline</v-icon>
              <p class="ma-2">10 GB storage</p>
          </v-row>
            <v-row class="ma-4">
              <v-icon>mdi-account-outline</v-icon>
              <p class="ma-2">Basic Support</p>
          </v-row>
         <v-container>
              <v-btn color="#9155fd" class="white--text" width="16em">Upgrade Plan</v-btn>
         </v-container>
          
        </v-card>
      </v-col>
       <v-btn class=" ma-3  mt-10 white--text" color="#9155fd"> save changes</v-btn>
        <v-btn class=" ma-3  mt-10 ml-2" outlined color="#adafb3">cancel</v-btn>
    </v-row>
  </v-card>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      show1: false,
      show2: true,
      show3: false,
      show4: false,
      password: "1234",
      rules: {},
    };
  },
};
</script>

<style>
</style>