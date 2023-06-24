<template>
  <ul class="dishes__items">
    <DishItem v-for="dish in dishes" :key="dish.id" :dish="dish" />
  </ul>
</template>

<script>
import dishes from '~/data/dishes'

export default {
  name: 'DishList',
  data () {
    return {
      page: 1,
      dishesPerPage: 3
    }
  },
  computed: {
    dishes () {
      const offset = (this.page - 1) * this.dishesPerPage
      return dishes.slice(offset, offset + this.dishesPerPage)
    }
  }
}
</script>
