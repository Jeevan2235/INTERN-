<template>
  <div>
    <v-container>
      
        <v-btn width="13em" elevation="0" color="#9155fd" class="white--text">
          Add Event
        </v-btn>
    
      <p class="mt-8">CALENDARS</p>

      <v-checkbox
        label="View All"
        v-model="ex4"
        color="#9155fd"
        hide-details
      ></v-checkbox>
      <v-checkbox
        label="Personal"
        v-model="ex4"
        color="#ff4c51"
        hide-details
      ></v-checkbox>
      <v-checkbox
        label="Business"
        v-model="ex4"
        color="#9155fd"
        hide-details
      ></v-checkbox>
      <v-checkbox
        label="Family"
        v-model="ex4"
        color="#ffb400"
        hide-details
      ></v-checkbox>
      <v-checkbox
        label="Holiday"
        v-model="ex4"
        color="#56ca00"
        hide-details
      ></v-checkbox
      ><v-checkbox
        label="ETC"
        v-model="ex4"
        color="#32bbff"
        hide-details
      ></v-checkbox>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>