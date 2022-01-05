<template>
  <div>
    <hello />
    <v-card width="65em" color="#f4f5fa">
   <common />
      <payment />
      <product/>
      <div class="text-center mt-16">
        <p style="font-size: 1.25rem; color: rgba(94,86,105,.87)">You still have a question?</p>
        <p>
          If you cannot find a question in our FAQ, you can always contact us.
          We will answer to you shortly!
        </p>
      </div>
     <help />
    </v-card>
  </div>
</template>

<script>
import hello from '~/components/hello.vue';
import Help from '~/components/help.vue';
import Payment from '~/components/payment.vue';
import Product from '~/components/product.vue';
export default {
  components: { hello, Payment, Product, Help },
  data: () => ({
    desserts: [
      {
        icon: "mdi-phone",
        title: "+ (810) 2548 2568",
        text: "We are always happy to help!",
      },
      {
        icon: "mdi-mail-outline",
        title: "hello@help.com",
        text: "Best way to get answer faster!",
      },
    ],
    
    items: [
      {
        title: "Does my subscription automatically renew?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "Can I store the item on an intranet so everyone has access?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "What does non-exclusive mean?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "Advanced Settings",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
    ],
    links: [
      {
        title: "Can I avail of an open delivery?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title:
          "I haven’t received the refund of my returned shipment. What do I do?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "How can I ship my order to an international location?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
      {
        title: "I missed the delivery of my order today. What should I do?",
        text: "Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.Donec placerat, lectus sed mattis semper, neque lectus feugiat lectus, varius pulvinar diam eros in elit. Pellentesque convallis laoreet laoreet.",
      },
    ],
  }),
};
</script>

<style>
</style>