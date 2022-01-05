<template>
  <div>
    <v-container>
      <h2>Chats</h2>
    </v-container>
    <v-row v-for="link in links" :key="link">
      <v-col cols="12" md="2">
        <v-avatar size="50">
          <v-img :src="link.img"></v-img>
        </v-avatar>
      </v-col>
      <v-col cols="12" md="7">
        <p>{{ link.text }}</p>
        <p>{{ link.text2 }}</p>
      </v-col>
      <v-col cols="12" md="3">
        <p>Dec 26</p>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        img: "1.png",
        text: "Gavin Griffith",
        text2: "I will purchase it for sure.",
      },
      {
        img: "2.png",
        text: "Harriet McBride",
        text2: "If it takes long you can..",
      },
    ],
  }),
};
</script>

<style>
</style>