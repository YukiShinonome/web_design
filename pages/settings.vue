<template>
  <v-card outlined>
    <v-card-title primary-title class="no_padding_bottom">設定</v-card-title>
    <v-card-text>
      <v-container fluid class="no_padding_top">
        <v-row>
          <v-col cols="12" sm="4" md="4">
            <v-switch label="ダークモード" v-model="$vuetify.theme.dark" hide-details></v-switch>
            <v-switch label="＊＊＊＊＊" hide-details></v-switch>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-switch label="indigo" color="indigo" value="indigo" hide-details></v-switch>
            <v-switch label="red" color="red" value="red" hide-details></v-switch>
          </v-col>
          <v-col cols="12" sm="4" md="4">
            <v-switch label="orange" color="orange" value="orange" hide-details></v-switch>
            <v-switch label="green" color="green" value="green" hide-details></v-switch>
          </v-col>
        </v-row>
      </v-container>
    </v-card-text>
  </v-card>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="scss" scoped>
.no_padding_top {
  padding-top: 0;
}
.no_padding_bottom {
  padding-bottom: 0;
}
</style>
