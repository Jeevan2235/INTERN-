<template>
  <v-card height="30em" width="78em" class="mt-16">
    <v-row>
      <v-col class="d-flex" cols="12" md="2" sm="6">
        <v-select :items="items" label="Actions" outlined disabled></v-select>
      </v-col>
      <v-btn height="4em" width="17em" color="#9155fd" class="white--text mt-3"
        >+ Create Invoice</v-btn
      >
      <v-spacer></v-spacer>
      <v-col cols="12" md="2">
        <v-text-field outlined label="Search Invoice"></v-text-field>
      </v-col>
      <v-col cols="12" md="2">
        <v-select outlined class="mr-4" label="Select Status"></v-select>
      </v-col>
    </v-row>
    <v-data-table
      :headers="headers"
      :items="data"
      :items-per-page="10"
      :single-select="singleSelect"
      show-select
      class="elevation-1"
    >
      <template v-slot:item.name="{ item }">
        <v-avatar size="30" class="mt-1">
          <img height="20" :src="item.avatar" />
        </v-avatar>
        <strong>
          {{ item.name }}
        </strong>
        <p class="pl-9">{{ item.mail }}</p>
      </template>
      <template v-slot:item.id="{ item }">
        <div>
          {{ item.id }}
        </div>
      </template>
      <template v-slot:item.icon="{ item }">
        <div>
          <v-btn rounded small fab elevation="0">
            <v-icon color="#57ca01" small>
              {{ item.icon }}
            </v-icon>
          </v-btn>
        </div>
      </template>
      <template v-slot:item.Actions="{ item }">
        <div>
          <v-icon>
            {{ item.Actions }}
          </v-icon>
          <v-icon>
            {{ item.Act }}
          </v-icon>
          <v-icon>
            {{ item.Acti }}
          </v-icon>
        </div>
      </template>
    </v-data-table>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    headers: [
      {
        align: "start",
        sortable: false,
      },
      { text: "#ID", value: "ID" },
      { text: "User", value: "icon" },
      { text: "Client", value: "name" },
      { text: "Total", value: "Total" },
      { text: "Date", value: "Date" },
      { text: "Balance", value: "Balance" },
      { text: "Actions", value: "Actions" },
    ],
    data: [
      {
        ID: "#4987",
        name: "Joseph Wheeler",
        mail: "pwillis@cross.org",
        Total: "$3428",
        Date: "2019-12-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "$724",
        icon: "mdi-check-circle-outline",
        avatar: "3.png",
      },
      {
        ID: "#4988",
        name: "Stephanie Burns",
        mail: "jamesjoel@chapman.net",
        Total: "$5219",
        Date: "	2019-07-17",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "Paid",
        icon: "mdi-download-circle-outline",
        avatar: "1.png",
      },
      {
        ID: "#4989",
        name: "Tony Herrera",
        mail: "eric47@george-castillo.com",
        Total: "$3542",
        Date: "2019-01-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "Paid",
        icon: "mdi-check-circle-outline",
        avatar: "1.png",
      },
      {
        ID: "#4990",
        name: "Kevin Patton",
        mail: "calvin07@joseph-edwards.org",
        Total: "$7826",
        Date: "2019-02-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "Paid",
        icon: "mdi-email-outline",
        avatar: "2.png",
      },
      {
        ID: "#4991",
        name: "Mrs. Julie Donovan MD",
        mail: "ywagner@jones.com",
        Total: "$7854",
        Date: "2019-07-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "$724",
        icon: "mdi-facebook",
        avatar: "3.png",
      },
      {
        ID: "#4992",
        name: "Amanda Phillips",
        mail: "john77@anderson.net",
        Total: "$9631",
        Date: "2019-02-23",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "Unpaid",
        icon: "mdi-check-circle-outline",
        avatar: "2.png",
      },
      {
        ID: "#4993",
        name: "Amanda Phillips",
        mail: "jeffrey25@martinez-hodge.com",
        Total: "$2365",
        Date: "2019-12-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "$724",
        icon: "mdi-facebook",
        avatar: "1.png",
      },
      {
        ID: "#4994",
        name: "Amanda Phillips",
        mail: "jeffrey25@martinez-hodge.com",
        Total: "$5465",
        Date: "2019-12-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "$724",
        icon: "mdi-check-circle-outline",
        avatar: "1.png",
      },
      {
        ID: "#4995",
        name: "Valerie Perez",
        mail: "jeffrey25@martinez-hodge.com",
        Total: "$5236",
        Date: "2019-12-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "Unpaid",
        icon: "mdi-download-circle-outline",
        avatar: "3.png",
      },
      {
        ID: "#4995",
        name: "Susan Dickerson",
        mail: "jeffrey25@martinez-hodge.com",
        Total: "$1256",
        Date: "2019-12-13",
        Actions: "mdi-delete-outline",
        Act: "mdi-eye-outline",
        Acti: "mdi-dots-vertical",
        Balance: "$724",
        icon: "mdi-download-circle-outline",
        avatar: "2.png",
      },
    ],
  }),
};
</script>
