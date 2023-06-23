<template>
    <div class="dishes__items">
        <div class="dishes__item" v-for="dish in dishes" :key="dish.id">
            <div class="dishes__price"><b>${{ dish.price }}</b></div>
            <nuxt-link to="/menu" class="dishes__link">
                <img :src="require(`~/assets/images/src/${dish.image}`)" :alt="dish.title" class="dishes__item-img">
            </nuxt-link>

            <div class="dishes__item-content">
                <div class="dishes__item-content-top">
                    <h3 class="dishes__item-content-title">{{ dish.title }}</h3>

                    <div class="dishes__form-counter">
                        <button class="dishes__minus-btn" type="button" aria-label="Убрать один товар">-</button>

                        <input class="dishes__input" type="text" value="+2" name="count">

                        <button class="dishes__plus-btn" type="button" aria-label="Добавить один товар">+</button>
                    </div>
                </div>

                <div class="dishes__item-content-down">
                    <div class="dishes__content-time">25 Min Away</div>
                </div>
            </div>
        </div>
       
    </div>
</template>

<script>
import dishes from '~/data/dishes';

export default {
    name: "Item",
    data() {
        return {
            dishes
        }
    }
}
</script>
