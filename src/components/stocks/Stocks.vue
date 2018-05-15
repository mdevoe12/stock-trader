<template lang="html">
  <div>
    <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
  </div>
</template>

<script>
import Stock from './Stock.vue'

export default {
  components: {
    appStock: Stock
  },
  data() {
    return {
      stocks: [
        { id: 1, name: 'BMW', price: 110 },
        { id: 2, name: 'Apple', price: 210 },
        { id: 3, name: 'Google', price: 90 },
        { id: 4, name: 'Twitter', price: 150 },
      ]
    }
  }
}
</script>

<style lang="css">
</style>
