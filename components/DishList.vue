<template>
  <ul class="dishes__items">
    <DishItem v-for="(dish, index) in dishes" :key="index" :dish="dish" />
  </ul>
</template>

<script>
import DishItem from './DishItem.vue'

export default {
  name: 'DishList',
  components: { DishItem },
  props: {
    dishes: {
      type: Array [String, Number, Boolean],
      required: true
    }
  }
}
</script>
