<template>
  <HomePage />
</template>

<script lang="ts">
import Vue from 'vue'
import HomePageVue from './HomePage.vue'

export default Vue.extend({
  name: 'IndexPage',
  components: { HomePage: HomePageVue }
})
</script>
