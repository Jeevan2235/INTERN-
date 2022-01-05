<template>
  <div>
    <v-row class="mt-10">
      <v-col cols="12" md="1">
        <v-chip class="ma-2" label text-color="white">
          <v-icon> mdi-help-circle-outline </v-icon>
        </v-chip>
      </v-col>
      <v-col>
        <p style="font-size: 1.25rem">Common</p>
        <p>Most asked questions.</p>
      </v-col>
    </v-row>

    <v-expansion-panels>
      <v-expansion-panel v-for="thing in things" :key="thing">
        <v-expansion-panel-header>
          {{ thing.title }}
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          {{ thing.text }}
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        title: "General Settings",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "Users",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "Personal Data",
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