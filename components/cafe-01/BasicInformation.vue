<template>
  <div>
    <div class="info-title text-center">BASIC INFORMATION</div>
    <v-container>
      <v-row>
        <v-col sm="4" md="4" class="info-item">
          <div class="text-center info-text">
            <span class="info-sub-title">営業時間</span>
            <br />10:00〜20:00
            <br />
            <span class="info-sub-title">定休日</span>
            <br />月曜日
            <br />
            <span class="info-sub-title">電話番号</span>
            <br />0000-11-2222
          </div>
        </v-col>
        <v-col sm="8" md="8">
          <v-img
            src="https://cdn.pixabay.com/photo/2017/08/07/07/06/coffeehouse-2600877_960_720.jpg"
          ></v-img>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style lang="scss" scoped>
.info-title {
  font-size: 1.3rem;
  padding: 20px 0 10px 0;
  margin: 0 20px;
  border-bottom: 2px solid #8b4513;
}

.info-item {
  align-self: center;
}

.info-text {
  vertical-align: middle;
  line-height: 2;
}

.info-sub-title {
  font-size: 1.1rem;
  font-weight: bold;
}
</style>
