<template>
  <v-row justify="center">
    <v-card class="mt-16" width="72em">
    <v-card elevation="4" tile>
      <v-row class="ml-4">
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
    <v-textarea
      label="Bio"
      height="5em"
      value="The name’s John Deo. I am a tireless seeker of knowledge, occasional purveyor of wisdom and also, coincidentally, a graphic designer. Algolia helps businesses across industries quickly create relevant 😎, scaLabel 😀, and lightning 😍 fast search and discovery experiences."
      outlined
      class="ma-8"
    ></v-textarea>
    <v-row class="ma-6">
      <v-col cols="12" md="6">
        <v-text-field
          label="Birthday"
          value="February 22, 1995"
          outlined
        ></v-text-field>
        <v-text-field
          label="Website"
          value="https://themeselection.com/"
          outlined
        ></v-text-field>
        <v-select
          label="Languages"
          value="February 22, 1995"
          outlined
        ></v-select>
       
      </v-col>
      <v-col cols="12" md="6">
        <v-text-field
          label="Phone"
          value="954-006-0844"
          outlined
        ></v-text-field>
        <v-select label="Country" value="February 22, 1995" outlined></v-select>
        <v-radio-group v-model="row" row>
          <v-radio color="#9155fd" label="Male" value="Male"></v-radio>
          <v-radio color="#9155fd" label="Female" value="Female"></v-radio>
          <v-radio color="#9155fd" label="Other" value="Other"></v-radio>
        </v-radio-group>
      </v-col>
       <v-btn class="white--text ma-3" color="#9155fd"> save changes</v-btn>
        <v-btn class="ma-3" outlined color="#adafb3">cancel</v-btn>
    </v-row>
    <v-row class="ml-5"> </v-row>
  </v-card>
  </v-row>
</template>

<script>
export default {};
</script>

<style>
</style>