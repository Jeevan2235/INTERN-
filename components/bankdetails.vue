<template>
  <v-row>
    <v-col cols="12" md="7" sm="4" v-for="link in links" :key="link">
      <p>{{ link.text }}</p>
      <p style="color: #cdcacf">{{ link.text1 }}</p>
      <p>{{ link.text2 }}</p>
      <p>{{ link.text3 }}</p>
      <p>{{ link.text4 }}</p>
      <p>{{ link.text5 }}</p>
    </v-col>
    <v-col cols="12" md="2" v-for="thing in things" :key="thing">
      <p>{{ thing.text }}</p>
      <p>{{ thing.text1 }}</p>
      <p>{{ thing.text2 }}</p>
      <p>{{ thing.text3 }}</p>
      <p>{{ thing.text4 }}</p>
      <p>{{ thing.text5 }}</p>
    </v-col>
    <v-col cols="12" md="3" v-for="item in items" :key="item">
      <p class="mt-10">{{ item.text }}</p>
      <p>{{ item.text1 }}</p>
      <p>{{ item.text2 }}</p>
      <p>{{ item.text3 }}</p>
      <p>{{ item.text4 }}</p>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        text: "Invoice To:",
        text1: "Jordan Stevenson",
        text2: "Hall-Robbins PLC",
        text3: "7777 Mendez Plains, USA",
        text4: "(616)865-4180",
        text5: "don85@johnson.com",
      },
    ],
    things: [
      {
        text: "Bill To:",
        text1: "Total Due:",
        text2: "Bank Name:",
        text3: "Country:",
        text4: "IBAN:",
        text5: "SWIFT Code:",
      },
    ],
    items: [
      {
        text: "$12,110.55",
        text1: "American Bank",
        text2: "United States",
        text3: "ETD95476213874685",
        text4: "(616)865-4180",
        text5: "BR91905",
      },
    ],
  }),
};
</script>

<style>
</style>