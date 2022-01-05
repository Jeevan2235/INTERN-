<template>
  <div class="mt-16">
    <v-card width="82em">
      <v-row>
        <v-col cols="12" md="3" sm="12">
          <v-container>
            <v-btn width="17em" color="#9155fd" class="white--text"
              >COMPOSE</v-btn
            >
          </v-container>
          <v-list>
            <v-list-item v-for="([icon, text], i) in items" :key="i" link>
              <v-list-item-icon>
                <v-icon>{{ icon }}</v-icon>
              </v-list-item-icon>

              <v-list-item-content>
                <v-list-item-title>{{ text }}</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
          <v-card-subtitle>LABELS</v-card-subtitle>
          <v-container>
            <v-list>
              <v-list-item-title v-for="link in links" :key="link" class="mt-4">
                <v-avatar size="10" class="ma-2" color="#ff4c51"></v-avatar>
                {{ link }}
              </v-list-item-title>
            </v-list>
          </v-container>
        </v-col>
        <v-divider vertical></v-divider>
        <v-col>
          <mail />
        </v-col>
      </v-row>
    </v-card>
  </div>
</template>

<script>
import mail from "~/components/mail.vue";
export default {
  components: { mail },
  data: () => ({
    items: [
      ["mdi-email", "Inbox"],
      ["mdi-send-outline", "Sent"],
      ["mdi-square-edit-outline", "Draft"],
      ["mdi-star-outline", "Starred"],
      ["mdi-incognito", "Spam"],
      ["mdi-trash-can", "Trash"],
    ],
    links: ["Personal", "Company", "Important", "Private"],
  }),
};
</script>

<style>
</style>
