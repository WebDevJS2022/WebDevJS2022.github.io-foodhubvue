<template>
    <div class="dishes__items">
        
        <DishItem v-for="dish in dishes" :key="dish.id" :dish="dish"/>
       
    </div>
</template>

<script>
import dishes from '~/data/dishes';

export default {
    name: 'DishList',
    data() {
        return {
            dishes
        }
    }
}
</script>
