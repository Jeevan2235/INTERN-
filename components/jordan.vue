<template>
  <v-row>
    <v-col cols="12" md="3" sm="12">
      <v-card-text style="font-weight: bold">Invoice To:</v-card-text>
      <v-select outlined label="Jordan Stevenson" :items="items"></v-select>
    </v-col>
    <v-spacer></v-spacer>

    <v-col cols="12" md="2" sm="6">
      <v-card-text style="font-weight: bold">Bill To:</v-card-text>
      <p>Total Due:</p>

      <p>Bank Name:</p>
      <p>Country:</p>
      <p>IBAN:</p>
      <p>SWIFT Code:</p>
    </v-col>
    <v-col cols="12" md="3" sm="6">
      <p class="mt-14">$12,110.55</p>
      <p>American Bank</p>
      <p>United States</p>
      <p>ETD95476213874685</p>
      <p>BR91905</p>
    </v-col>
  </v-row>
</template>

<script>
export default {};
</script>

<style>
</style>