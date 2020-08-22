<template>
  <div class="container">
    <v-tabs grow background-color="transparent" color="#000" slider-color="#8b4513">
      <v-tab>home</v-tab>
      <v-tab>menu</v-tab>
      <v-tab>access</v-tab>
      <v-tab>contact</v-tab>
    </v-tabs>
    <v-img
      src="https://cdn.pixabay.com/photo/2016/02/03/17/29/coffee-1177533_960_720.jpg"
      max-height="500px"
    ></v-img>
    <div class="news-title text-center">NEWS</div>
    <v-simple-table class="table-margin" height="300px">
      <tbody>
        <tr v-for="(item, idx) in items" :key="idx">
          <td>{{ item.category }}</td>
          <td>{{ item.content }}</td>
        </tr>
      </tbody>
    </v-simple-table>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data: () => ({
    items: [
      {
        category: 'お知らせ',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'お知らせ',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'メニュー',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'お知らせ',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'メニュー',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'お知らせ',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'お知らせ',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      },
      {
        category: 'メニュー',
        content:
          'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor'
      }
    ]
  })
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

.news-title {
  font-size: 1.2rem;
  padding: 20px 0 10px 0;
  margin: 0 20px;
  border-bottom: 2px solid #8b4513;
}

.theme--light.v-data-table {
  background-color: transparent;
  margin: 0 20px;
}
</style>
