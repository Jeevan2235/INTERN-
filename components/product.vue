<template>
  <div>
    <v-row class="mt-10">
      <v-col cols="12" md="1">
        <v-chip class="ma-2" label text-color="white">
          <v-icon> mdi-bag-checked </v-icon>
        </v-chip>
      </v-col>
      <v-col>
        <p style="font-size: 1.25rem">Product & Services</p>
        <p>Product related questions.</p>
      </v-col>
    </v-row>
    <v-expansion-panels>
      <v-expansion-panel v-for="link in links" :key="link">
        <v-expansion-panel-header>
          {{ link.title }}
        </v-expansion-panel-header>
        <v-expansion-panel-content>
          {{ link.text }}
        </v-expansion-panel-content>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        title: "Can I avail of an open delivery?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title:
          "I haven’t received the refund of my returned shipment. What do I do?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "How can I ship my order to an international location?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "I missed the delivery of my order today. What should I do?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
    ],
  }),
};
</script>

<style>
</style>