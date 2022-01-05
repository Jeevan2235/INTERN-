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
      <div class="mt-10 ma-8">
        <v-row>
          <v-icon class="ma-3">mdi-chart-timeline-variant</v-icon>
          <p class="mt-3" style="font-weight: 500; font-size: 1.25rem">
            Activity
          </p>
        </v-row>
        <v-row v-for="thing in things" :key="thing">
          <v-col md="1" sm="2"><v-switch color="#9155fd"></v-switch></v-col>
          <v-col md="11" sm="12">
            <p class="mt-5">
              {{ thing.text }}
            </p></v-col
          >
        </v-row>
        <v-row class="mt-10">
          <v-icon class="ma-3">mdi-email-outline</v-icon>
          <p class="mt-3" style="font-weight: 500; font-size: 1.25rem">
            Application
          </p>
        </v-row>
        <v-row v-for="link in links" :key="link">
          <v-col md="1" sm="2"><v-switch color="#9155fd"></v-switch></v-col>
          <v-col md="11" sm="12">
            <p class="mt-5">
              {{ link.text }}
            </p></v-col
          >
        </v-row>

        <v-btn class="ma-3 mt-8 white--text" color="#9155fd">
          save changes</v-btn
        >
        <v-btn class="ma-3 mt-8" outlined color="#adafb3">cancel</v-btn>
      </div>
    </v-card>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        text: "E-mail me when someone comments on my article",
      },
      {
        text: "E-mail me when someone follows me",
      },
      {
        text: "E-mail me when someone answers on my forum thread",
      },
    ],
    links: [
      {
        text: "News and Announcements",
      },
      {
        text: "Weekly product updates",
      },
      {
        text: "Weekly blog digest",
      },
    ],
  }),
};
</script>

<style>
</style>