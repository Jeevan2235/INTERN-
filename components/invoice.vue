<template>
   <v-row>
            <v-col cols="12" md="3">
              <p style="font-weight: bold">Invoice To:</p>
              <v-select
                outlined
                label="Jordan Stevenson"
                :items="items"
              ></v-select>
              <p style="color: #cdcacf">Jordan Stevenson</p>
              <p>Hall-Robbins PLC</p>
              <p>7777 Mendez Plains, USA</p>
              <p>(616)865-4180</p>
              <p>don85@johnson.com</p>
            </v-col>
            <v-spacer></v-spacer>

            <v-col cols="12" md="2">
              <p style="font-weight: bold">Bill To:</p>
              <p>Total Due:</p>
              <p>Bank Name:</p>
              <p>Country:</p>
              <p>IBAN:</p>
              <p>SWIFT Code:</p>
            </v-col>
            <v-col cols="12" md="3">
              <p class="mt-10">$12,110.55</p>
              <p>American Bank</p>
              <p>United States</p>
              <p>ETD95476213874685</p>
              <p>BR91905</p>
            </v-col>
          </v-row>
</template>

<script>
export default {

}
</script>

<style>

</style>