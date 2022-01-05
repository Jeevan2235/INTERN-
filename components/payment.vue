<template>
  <div>
    <v-row class="mt-10">
      <v-col cols="12" md="1">
        <v-chip class="ma-2" label text-color="white">
          <v-icon> mdi-currency-usd </v-icon>
        </v-chip>
      </v-col>
      <v-col>
        <p style="font-size: 1.25rem">Payment</p>
        <p>Payment methods questions.</p>
      </v-col>
    </v-row>
    <v-expansion-panels>
      <v-expansion-panel v-for="item in items" :key="item">
        <v-expansion-panel-header>
          {{ item.title }}
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          {{ item.text }}
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      {
        title: "Does my subscription automatically renew?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "Can I store the item on an intranet so everyone has access?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "What does non-exclusive mean?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "Advanced Settings",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
    ],
  }),
};
</script>

<style>
</style>