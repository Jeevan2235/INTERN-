<template>
  <div class="mt-16">
    <v-row justify="center">
      <v-card width="70em">
      <p
        class="text-center"
        style="
          font-size: 2rem;
          font-weight: 500;
          color: rgba(94, 86, 105, 0.87);
        "
      >
        Pricing Plans
      </p>
      <p class="text-center" style="color: rgba(94, 86, 105, 0.87)">
        All plans include 40+ advanced tools and features to boost your product.
        Choose the <br />
        best plan to fit your needs.
      </p>
      <v-row justify="center">
        <v-col md="1">
          <p
            class="text-center mt-5"
            style="font-weight: 600; color: rgba(94, 86, 105, 0.87)"
          >
            Monthly
          </p></v-col
        >
        <v-col md="1">
          <v-switch v-model="sticky" hide-details class="ml-4" color="#9155fd"></v-switch
        ></v-col>
        <v-col md="1">
          <p
            class="text-center mt-5"
            style="font-weight: 600; color: rgba(94, 86, 105, 0.87)"
          >
            Anually
          </p></v-col
        >
      </v-row>
      <v-row justify="center">
        <v-card
          v-for="link in links"
          :key="link"
          class="ma-3"
          elevation="0"
          outlined
        >
          <v-container>
            <v-img :src="link.img"></v-img>
            <p
              class="text-center"
              style="font-size: 1.5rem;     color: rgba(94,86,105,.87; font-weight: 500"
            >
              {{ link.title }}
            </p>
            <p class="text-center" style="color: rgba(94, 86, 105, 0.87)">
              {{ link.text }}
            </p>
            <p class="text-center" style="font-size: 2rem; color:#9155fd">{{ link.rate }}</p>
            <v-row>
              <v-icon></v-icon>
              <p></p>
            </v-row>
            <v-list>
              <v-list-item v-for="(item, i) in items" :key="i">
                <v-list-item-content>
                  <v-list-item-title style="color: rgba(94, 86, 105, 0.87)">{{
                    item
                  }}</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list>
            <div class="text-center">
              <v-btn
                elevation="0"
                color="#9574d8"
                width="18em"
                class="white--text mt-3 mb-3"
                >{{ link.btn }}</v-btn
              >
            </div>
          </v-container>
        </v-card>
      </v-row>
      <div class="mt-16">
        <v-card elevation="0" outlined tile color="#f9f8f9">
           <v-container>
          <v-row>
        
              <v-col  cols="12" md="6">
              <p style="color: #9574d8; font-size: 1.5rem">
                Still not convinced? Start with a 14-day FREE trial!
              </p>
              <p style="color: rgba(94, 86, 105, 0.87)">
                You will get full access to with all the features for 14 days.
              </p>
              <v-btn color="#9574d8" class="white--text mb-6"
                >Start 14-day free trial</v-btn
              >
            </v-col>
            <v-col cols="12" md="5">
              <v-img src="13.png" width="50%" style="margin-top: -40px"></v-img>
            </v-col>
        
          </v-row>
           </v-container>
        </v-card>
        <div class="mt-16 text-center">
          <h3 style="color: rgba(94, 86, 105, 0.87)">FAQ's</h3>
          <p style="color: rgba(94, 86, 105, 0.87)">
            Let us help answer the most common questions.
          </p>
          <v-container>
            <v-expansion-panels>
              <v-expansion-panel v-for="thing in things" :key="thing">
                <v-expansion-panel-header
                  style="color: rgba(94, 86, 105, 0.87)"
                >
                  {{ thing.title }}
                </v-expansion-panel-header>
                <v-expansion-panel-content
                  style="color: rgba(94, 86, 105, 0.87)"
                >
                  {{ thing.text }}
                </v-expansion-panel-content>
              </v-expansion-panel>
            </v-expansion-panels>
          </v-container>
        </div>
      </div>
    </v-card>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      " 100 responses a month",
      "Unlimited forms and surveys",
      "Unlimited fields",
      "Basic form creation tools",
      "Up to 2 subdomains",
    ],

    links: [
      {
        img: "10.png",
        title: "Basic",
        rate: "$0/month",
        text: "A simple start for everyone",
        text2: "100 responses a month",

        btn: "Your Current Plan",
      },
      {
        img: "11.png",
        rate: "$49/month",
        title: "Standard",
        text: "For small to medium businesses",

        btn: "Upgrade",
      },
      {
        img: "12.png",
        rate: "$49/month",
        title: "Enterprise",
        text: "Solution for big organizations",

        btn: "Upgrade",
      },
    ],
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