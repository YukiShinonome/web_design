<template>
  <div class="container">
    <v-tabs grow background-color="transparent" color="#8b4513" slider-color="#8b4513">
      <v-tab>home</v-tab>
      <v-tab>menu</v-tab>
      <v-tab>access</v-tab>
    </v-tabs>
    <v-img
      src="https://cdn.pixabay.com/photo/2016/02/03/17/29/coffee-1177533_960_720.jpg"
      max-height="500px"
    ></v-img>
    <News></News>
    <BasicInfo></BasicInfo>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import News from '~/components/cafe-01/News.vue'
import BasicInfo from '~/components/cafe-01/BasicInformation.vue'

export default Vue.extend({
  components: {
    News,
    BasicInfo
  }
})
</script>

<style lang="scss" scoped>
.container {
  background-color: #faebd7;
}

.v-tabs {
  margin-bottom: 10px;
}

.v-tab {
  font-size: 1.2rem;
}
</style>
