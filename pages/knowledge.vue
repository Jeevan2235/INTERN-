<template>
  <div >
    <v-row justify="center">
      <hello />
       </v-row>

    <v-row justify="center">
      <v-card width="24em" class="mt-16 ma-3" v-for="link in links" :key="link">
        <v-card tile elevation="0" color="#fafafa">
          <v-row justify="center" class="mt-6">
          <v-img :src="link.img" max-height="220" max-width="140"></v-img>
        </v-row>
        </v-card>
        <p
          class="text-center mt-6"
          style="font-size: 1.25rem; letter-spacing: 0.0125em"
        >
          {{ link.title }}
        </p>
        <v-card-text class="text-center" >{{ link.text }}</v-card-text>
      </v-card>
    </v-row>
   
  </div>
</template>

<script>
import hello from "~/components/hello.vue";
export default {
  components: { hello },
  data: () => ({
    links: [
      {
        img: "7.png",
        title: "Sales Automation 👩🏻‍💻",
        text: "There is perhaps no better demonstration of the folly of image of our tiny world.",
      },
      {
        img: "9.png",
        title: "Marketing Automation 🚀",
        text: "Look again at that dot. That’s here. That’s home. That’s us. On it everyone you love.",
      },
      {
        img: "8.png",
        title: "API Questions 📱",
        text: "Every hero and coward, every creator and destroyer of civilization.",
      },
      {
        img: "7.png",
        title: "Email Marketing ✉️",
        text: "There is perhaps no better demonstration of the folly of human conceits.",
      },
      {
        img: "8.png",
        title: "Personalization 🤩",
        text: "It has been said that astronomy is a humbling and character experience.",
      },
      {
        img: "9.png",
        title: "Demand Generation 🤟🏻",
        text: "Competent means we will never take anything for granted.",
      },
    ],
  }),
};
</script>

<style>
</style>