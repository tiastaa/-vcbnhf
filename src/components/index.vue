<template>
    <div class="list-container">
        <product-card
            v-for="item in productListData"
            :key="item.id"
            :img-src="item.imgSrc"
            :title="item.title"
        />
    </div>
</template>

<script >
import ProductCard from './ProductCard.vue'
export default {
    name: 'ProductList',
    components: {
    ProductCard,
  },

  props: {
    productListData: {
      type: Array,
      default: () => [],
    },
  },
}

</script>

<style scoped>
.list-container{
    display: flex;
    justify-content: center;
}
</style>