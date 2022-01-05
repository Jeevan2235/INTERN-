<template>
  <div>
    <v-card width="75em">
      <v-row>
        <v-col cols="12" md="3">
          <add />
        </v-col>
        <v-divider vertical></v-divider>
        <v-col cols="12" md="9">
          <calendarw />
        </v-col>
      </v-row>
    </v-card>
  </div>
</template>

<script>
import add from "~/components/add.vue";
import Calendarw from "~/components/calendarw.vue";
export default {
  components: { add, Calendarw },
};
</script>

<style></style>
