<template>
 <div>
    <v-row>
    <v-col cols="12" md="7" sm="12">
      <v-card  width="55em">
        <v-container>
          <materio />
          <v-divider></v-divider>
          <jordan />
        </v-container>
        <v-divider></v-divider>
        <item-3 />
        <v-divider></v-divider>
      <salesperson-3 />
      </v-card>
    </v-col>
    <v-col cols="12" md="5" sm="12">
   <sendinvoice />
    </v-col>
  </v-row>
 </div>
</template>

<script>
import Jordan from "~/components/jordan.vue";
import materio from "~/components/materio.vue";
import Salesperson3 from '~/components/salesperson3.vue';
import Sendinvoice from '~/components/sendinvoice.vue';
export default {
  components: { materio, Jordan, Salesperson3, Sendinvoice },
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
