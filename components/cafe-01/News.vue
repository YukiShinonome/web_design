<template>
  <div>
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
.news-title {
  font-size: 1.5rem;
  padding: 20px 0 10px 0;
  margin: 0 20px;
  border-bottom: 2px solid #8b4513;
  font-family: 'Fredericka the Great', sans-serif;
}

.theme--light.v-data-table {
  background-color: transparent;
  margin: 0 20px;
}
</style>
