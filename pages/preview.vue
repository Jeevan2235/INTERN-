<template>
  <v-row>
    <v-col cols="12" md="8">
      <v-card  width="60em">
        <v-container>
          <materio />
          <v-divider></v-divider>
          <bankdetails />
        </v-container>
        <v-divider></v-divider>
        <item />
        <v-divider></v-divider>
        <v-container>
          <salesperson />
          <v-divider></v-divider>
          <v-card-text
            class="pr-16"
            style="color=#9f9aa5"
            >Note: It was a pleasure working with you and your team. We hope you
            will keep us in mind for future freelance projects. Thank
            You!</v-card-text
          >
        </v-container>
      </v-card>
    </v-col>
    <v-col cols="12" md="4">
      <v-card height="16em" width="20em" elevation="1">
        <v-container>
          <v-btn width="21em" color="#9155fd" class="white--text"
            ><v-icon>mdi-send-outline</v-icon>
            <p class="mt-4 pa-2">Send Invoice</p>
          </v-btn>
          <v-btn width="21em" class="mt-3">DOWNLOAD</v-btn>
          <v-btn width="21em" class="mt-3">PRINT</v-btn>
          <v-btn width="21em" class="mt-3">EDIT INVOICE</v-btn>
          <v-btn width="21em" class="mt-3 white--text" color="#56ca00"
            ><v-icon>mdi-currency-usd</v-icon>
            <p class="mt-4 pa-2">Add Payment</p></v-btn
          >
        </v-container>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import Bankdetails from "~/components/bankdetails.vue";
import Item from "~/components/item.vue";
import materio from "~/components/materio.vue";
import Salesperson from "~/components/salesperson.vue";
export default {
  components: { materio, Bankdetails, Item },
};
</script>

<,
    Salespersonstyle></style>
