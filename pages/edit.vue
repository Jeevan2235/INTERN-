<template>
  <v-row>
    <v-col cols="12" md="7">
      <v-card  width="55em">
        <v-container>
          <materio />
          <v-divider></v-divider>
          <invoice />
        </v-container>
        <v-divider></v-divider>
        <item-2 />
        <v-divider></v-divider>
        <salesperson-2 />
      </v-card>
    </v-col>
  <payment-2 />
  </v-row>
</template>

<script>
import Invoice from "~/components/invoice.vue";
import Item2 from "~/components/item2.vue";
import materio from "~/components/materio.vue";
import Payment2 from '~/components/payment2.vue';
import Salesperson2 from "~/components/salesperson2.vue";
export default {
  components: { materio, Invoice, Item2, Salesperson2, Payment2 },
  data: () => ({
    items: [
      "Stephanie Burns",
      "Tony Herrera",
      "Kevin Patton",
      "Mrs. Julie Donovan MD",
    ],

    things: [
      "App Design",
      "App Customization",
      "ABC Template",
      "App Development",
    ],
  }),
};
</script>

<style></style>
