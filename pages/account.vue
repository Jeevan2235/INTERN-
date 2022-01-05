<template>
  <v-row justify="center">
    <v-card class="mt-16" width="72em">
    <v-card elevation="4" tile>
      <v-row class="ml-2">
        <v-btn height="3em" class="ma-2" tile color="white" elevation="0" >
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
    <accountcontent />
  </v-card>
  </v-row>
</template>

<script>
import accountcontent from "~/components/accountcontent.vue";
export default {
  components: { accountcontent },
  data: () => ({
    links: ["Active", "Inactive", "Pending", "Closed"],
  }),
};
</script>

<style>
</style>