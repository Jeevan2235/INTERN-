<template>
    <v-row justify="center">
      <v-card class="mt-16 ml-16" width="72em">
    <v-card elevation="4" tile>
      <v-row class="ml-4">
        <v-btn height="3em" class="ma-2 ml-3" tile color="white" elevation="0" >
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
    <securitycontent />
    </v-card>
    </v-row>
</template>

<script>
import securitycontent from '~/components/securitycontent.vue'
export default {
  components: { securitycontent },

}
</script>

<style>

</style>