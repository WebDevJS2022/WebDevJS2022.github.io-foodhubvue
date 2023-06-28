<template>
  <ul class="dishes__pagination">
    <li class="dishes__pagination-item">
      <button
        class="dishes__pagination-link pagination__link--arrow"
        :disabled="page === 1"
        aria-label="Предыдущая страница"
        @click.prevent="prevPage()"
      >
        <img src="~/assets/images/src/arrowleft.png" alt="" class="dishes__pagination-img">
      </button>
    </li>
    <li v-for="pageNumber in pages" :key="pageNumber" class="dishes__pagination-item">
      <a
        href="#"
        class="dishes__pagination-link pagination__link--current"
        :class="{'pagination__link--current': pageNumber === page}"
        @click.prevent="paginate(pageNumber)"
      >
        {{ pageNumber }}
      </a>
    </li>

    <li class="dishes__pagination-item">
      <button
        class="dishes__pagination-link pagination__link--arrow"
        :disabled="page === 2"
        href="#"
        aria-label="Следующая страница"
        @click.prevent="nextPage()"
      >
        <img src="~/assets/images/src/arrowright.png" alt="" class="dishes__pagination-img">
      </button>
    </li>
  </ul>
</template>

<script>

export default {
  name: 'BasePagination',
  model: {
    prop: 'page',
    event: 'paginate'
  },
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
  },
  methods: {
    paginate (page) {
      this.$emit('paginate', page)
    },
    nextPage () {
      this.$emit('paginate', (this.page + 1))
    },
    prevPage () {
      this.$emit('paginate', (this.page - 1))
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
    display: flex;
    justify-content: center;
    align-items: center;
  width: 5rem;
  height: 5rem;
  font-size: 3rem;
  font-weight: 600;
  line-height: 2rem;
  color: #a8a8a8;
  margin-right: 2rem;
}
.dishes__pagination-link {
  cursor: pointer;
  color: #a8a8a8;
  border: none;
  background-color: inherit;
}
</style>
