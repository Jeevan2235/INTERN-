<template>
  <div>
    <v-row>
      <v-col md="12" sm="12">
        <v-container>
          <v-row
            ><v-icon class="ma-3">mdi-magnify </v-icon>
            <v-text-field label="search..."></v-text-field>
          </v-row>
        </v-container>

        <v-row>
          <v-checkbox class="ma-4"> </v-checkbox>
          <v-icon class="mb-4 pr-2">mdi-trash-can-outline</v-icon>
          <v-icon class="mb-4 pr-2">mdi-email-open-outline</v-icon>
          <v-icon class="mb-4 pr-2">mdi-folder-outline</v-icon>
          <v-icon class="mb-4 pr-2">mdi-label-outline</v-icon>

          <v-spacer></v-spacer>

          <v-btn class="mx-2" fab small elevation="0" color="white">
            <v-icon dark> mdi-reload </v-icon>
          </v-btn>
          <v-btn fab small elevation="0" color="white" class="mr-5">
            <v-icon>mdi-dots-vertical</v-icon></v-btn
          >
        </v-row>

        <v-divider></v-divider>

        <v-card tile v-for="link in links" :key="link">
          <v-row>
            <v-checkbox color="#9155fd" class="ma-4"></v-checkbox>
            <v-rating length="1" class="mt-3" color="orange"></v-rating>
            <v-avatar size="30" class="mt-3 ma-3">
              <v-img :src="link.img"></v-img>
            </v-avatar>
            <p class="mt-4 ma-5">{{ link.name }}</p>
            <v-btn
              height="15px"
              elevation="0"
              rounded
              class="mt-5 ma-3"
              style="color: #90db59"
              small
              >{{ link.btn }}</v-btn
            >
            <v-btn
              height="15px"
              elevation="0"
              rounded
              class="mt-5 ma-3"
              style="color: #9155fd"
              small
              >{{ link.btn2 }}</v-btn
            >
            <p class="mt-4 ml-5" style="font-size: 14px">{{ link.text }}</p>
            <v-spacer></v-spacer>
            <p class="mt-4 ma-4 pr-3">{{ link.date }}</p>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        btn: "IMPORTANT",
        date: "Jul 22",
        btn2: "COMPANY",
        name: "Charles Cooper",
        img: "1.png",
        text: "Amount collection marriage price.",
      },
      {
        btn: "Company",
        date: "Jul 22",
        img: "2.png",
        name: "Lindsey Melton",
        text: "Simply idea project health prevent beyond both after.",
      },
      {
        btn: "Personal",
        date: "Jul 22",
        img: "3.png",
        btn2: "Company",
        name: "Jennifer Garcia",
        text: "Green attorney government same course join in woman.",
      },
      {
        btn: "Private",
        date: "Jul 22",
        img: "2.png",
        name: "Kathryn Smith",
        text: "Test look option movement position card cause.",
      },

      {
        btn: "Private",
        date: "Jul 22",
        img: "1.png",
        name: "Lindsey Melton",
        text: "Always beautiful name push miss international.",
      },
      {
        btn: "Personal",
        date: "Jul 22",
        btn2: "Private",
        img: "2.png",
        name: "Lindsey Melton",
        text: "Apply loss always difference husband course deal.",
      },

      {
        btn: "Important",
        date: "Jul 22",
        btn2: "Personal",
        img: "3.png",
        name: "Lindsey Melton",
        text: "Over tough city well first should quite.",
      },
      {
        btn: "Important",
        date: "Jul 22",
        btn2: "Personal",
        img: "3.png",
        name: "Lindsey Melton",
        text: "Over tough city well first should quite.",
      },
    ],
  }),
};
</script>

<style lang="sass" scoped>
.v-card.on-hover.theme--dark
  background-color: rgba(#FFF, 0.8)
  >.v-card__text
    color: #000
</style>
