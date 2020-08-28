<template>
  <div class="container">
    <v-tabs
      grow
      background-color="transparent"
      color="#8b4513"
      slider-color="#8b4513"
    >
      <v-tab>home</v-tab>
      <v-tab>menu</v-tab>
      <v-tab>access</v-tab>
    </v-tabs>
    <v-img
      src="https://source.unsplash.com/mpSMThAU4OY"
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
  font-size: 1.5rem;
  font-family: 'Fredericka the Great', sans-serif;
  /* font-weight: bold; */
}

.v-image {
  position: relative;
  &::after {
    position: absolute;
    bottom: 0;
    left: 20px;
    line-height: 1;
    content: 'Shinonome Cafe';
    font-size: 7rem;
    font-family: 'Fredericka the Great', sans-serif;
    color: #fff;
  }
}
</style>
