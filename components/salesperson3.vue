<template>
  <div>
        <v-container>
          <v-row>
            <v-col cols="12" md="5">
              <v-row>
                <p class="mt-5">Salesperson:</p>
                <v-text-field
                  label="Tom Cook"
                  outlined
                  class="ma-2"
                ></v-text-field>
              </v-row>
              <v-text-field
                label="Thanks for your business"
                outlined
              ></v-text-field>
            </v-col>
            <v-spacer></v-spacer>
            <v-col cols="12" md="2">
              <p>Subtotal:</p>
              <p>Discount:</p>
              <p>Tax:</p>
              <v-divider></v-divider>
              <p>Total:</p>
            </v-col>

            <v-col cols="12" md="2">
              <p>$1800</p>
              <p>$28</p>
              <p>21%</p>
              <v-divider></v-divider>
              <p>$1690</p>
            </v-col>
          </v-row>
          <v-divider></v-divider>
          <v-card-text class="pr-16" style="color=#9f9aa5">Note: </v-card-text>
          <v-textarea
            outlined
            height="30"
            label="It was a pleasure working with you and your team. We hope you
            will keep us in mind for future freelance projects. Thank
            You!"
          ></v-textarea>
        </v-container>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>