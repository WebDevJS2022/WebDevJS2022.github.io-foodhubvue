<template>
  <ul class="dishes__pagination">
    <li class="dishes__pagination-item">
      <a
        class="dishes__pagination-link pagination__link--arrow pagination__link--disabled"
        aria-label="Предыдущая страница"
      >
        <img src="~/assets/images/src/arrowleft.png" alt="" class="dishes__pagination-img">
      </a>
    </li>
    <li v-for="pageNumber in pages" :key="pageNumber" class="dishes__pagination-item">
      <a
        class="dishes__pagination-link pagination__link--current"
        :class="{'pagination__link--current': pageNumber === page}"
      >
        {{ pageNumber }}
      </a>
    </li>

    <li class="dishes__pagination-item">
      <a class="dishes__pagination-link pagination__link--arrow" href="#" aria-label="Следующая страница">
        <img src="~/assets/images/src/arrowright.png" alt="" class="dishes__pagination-img">
      </a>
    </li>
  </ul>
</template>

<script>

export default {
  name: 'BasePagination',
  props: {
    page: {
      type: Number,
      default: 1
    },
    count: {
      type: Number,
      required: true
    },
    perPage: {
      type: Number,
      default: 3
    }
  },
  computed: {
    pages () {
      return Math.ceil(this.count / this.perPage)
    }
  }
}
</script>

<style scoped>
.dishes__pagination {
  display: flex;
  width: 30rem;
  margin: 10rem auto 0;
}
.dishes__pagination-item {
  width: 5rem;
  height: 5rem;
  font-size: 3rem;
  font-weight: 600;
  line-height: 2rem;
  color: #a8a8a8;
}
.dishes__pagination-link {
  color: #a8a8a8;
}
</style>
