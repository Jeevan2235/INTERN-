<template>
  <div>
      <v-container>
          <h2>Contacts</h2>
        </v-container>
         <v-row v-for="thing in things" :key="thing">
          <v-col cols="12" md="2">
            <v-avatar size="50" >
              <v-img :src="thing.img"></v-img>
            </v-avatar>
          </v-col>
          <v-col cols="12" md="10">
          
            <p>{{thing.text}}</p>
            <p>{{thing.text2}}</p>
          </v-col>
         
        </v-row>
  </div>
</template>

<script>
export default {
     data: () => ({

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

};
</script>

<style>

</style>