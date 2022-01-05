<template>
  <div>
    <v-row>
      <v-col  md="6" sm="12">
        <v-card-text style="font-weight: bold">ITEM</v-card-text>
      </v-col>

      <v-col  md="2" sm="12">
        <v-card-text style="font-weight: bold">COST</v-card-text>
      </v-col>
      <v-col  md="2" sm="12">
        <v-card-text style="font-weight: bold">HOURS</v-card-text>
      </v-col>
      <v-col  md="2" sm="12">
        <v-card-text style="font-weight: bold">PRICE</v-card-text>
      </v-col>
    </v-row>
    <v-container>
      <v-card  width="53em" class="pa-5" elevation="0" outlined>
        <v-row>
          <v-col  md="6" sm="12">
            <v-select outlined label="Select Item" :items2="items2"></v-select>
            <v-textarea outlined height="80" label="Description"></v-textarea>
          </v-col>
          <v-col  md="2" sm="12">
            <v-select outlined label="Cost"></v-select>
          </v-col>
          <v-col  md="2" sm="12">
            <v-select outlined label="Hours"></v-select>
          </v-col>
          <v-col  md="2" sm="12">
            <v-card-text>$0</v-card-text>
          </v-col>
        </v-row>
      </v-card>
      <v-btn class="mt-3 mb-7" elevation="0" outlined color="#9155fd"
        >ADD-ITEM</v-btn
      >
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>