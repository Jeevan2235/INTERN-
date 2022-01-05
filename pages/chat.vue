<template>
  <div class="mt-16">
    <v-container>
      <v-card height="40em" width="24em">
        <v-row justify="center" align="center"> </v-row>
        <v-container
          id="scroll-target"
          style="max-height: 620px"
          class="overflow-y-auto"
        >
        <v-row >
          <v-col cols="12" md="2">
            <v-avatar size="50" class="mt-5">
               <v-img src="2.png"></v-img>
            </v-avatar>
</v-col>
<v-col cols="12" md="10">
  <v-text-field rounded outlined class="mt-5" label="search.." >
    <v-icon>mdi-facebook</v-icon>
  </v-text-field>
</v-col>
        </v-row>

        
        <v-divider></v-divider>
        <chats />
        <contacts />
          <v-row
            v-scroll:#scroll-target="onScroll"
            align="center"
            justify="center"
           
          >
          </v-row>
        </v-container>
      </v-card>
    </v-container>
  </div>
</template>

<script>
import chats from '~/components/chats.vue';
import Contacts from '~/components/contacts.vue';
export default {
  components: { chats, Contacts },
  data: () => ({
    links:[{
      img: "1.png",
      text:"Gavin Griffith",
      text2:"I will purchase it for sure.",
    },
    {
      img: "2.png",
      text:"Harriet McBride",
      text2:"If it takes long you can..",
    }],

    things:[{
      img: "3.png",
      text:"Gavin Griffith",
      text2:"We need to check if we can provide..",
    },
    {
      img: "1.png",
      text:"Harriet McBride",
      text2:"If it takes long you can help us make..",
    },
    {
      img: "2.png",
      text:"Danny Conner",
      text2:"We need to check if we can provide..",
    },
    {
      img: "1.png",
      text:"Janie West",
      text2:"If it takes long you can help us make..",
    },
    {
      img: "3.png",
      text:"Bryan Murray",
      text2:"We need to check if we can provide..",
    },
    {
      img: "2.png",
      text:"Albert Underwood",
      text2:"If it takes long you can help us make..",
    },
    {
      img: "1.png",
      text:"Adele Ross",
      text2:"We need to check if we can provide..",
    }]
  }),

  methods: {
    onScroll(e) {
      this.offsetTop = e.target.scrollTop;
    },
  },
};
</script>