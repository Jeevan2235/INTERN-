<template>
  <div>
    <v-card height="10em" width="18em" elevation="1">
      <v-container>
        <v-btn width="19em" color="#9155fd" class="white--text"
          ><v-icon>mdi-send-outline</v-icon>
          <p class="mt-4 pa-2">Send Invoice</p>
        </v-btn>
        <v-btn width="19em" class="mt-3" outlined>PREVIEW</v-btn>
        <v-btn width="19em" class="mt-3" outlined>SAVE</v-btn>
      </v-container>
    </v-card>
    <v-card width="18em" class="mt-4 pa-3">
      <v-select outlined label="Accept Payment Via"></v-select>
      <v-card-text>Payment Terms</v-card-text>
      <v-card-text>Client Notes</v-card-text>
      <v-card-text>Payment Stub</v-card-text>
    </v-card>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>