<template>
  <div class="product-grid">
    <div v-for="product in products" :key="product.id" class="product-card">
      <img :src="product.image" :alt="product.name" class="product-image" />
      <h3 class="product-name">{{ product.name }}</h3>
      <p class="product-price">{{ product.content }}</p>
    </div>
  </div>
</template>


<script>
export default {
  props: {
    products: {
      type: Array,
      required: true,
    },
  },
  methods: {
    // formatPrice(price) {
    //   return `$${price.toFixed(2)}`
    // },
  },
}
</script>

<style scoped>
.product-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
}

.product-card {
  border: 1px solid #ccc;
  border-radius: 5px;
  padding: 16px;
  width: 200px;
  text-align: center;
}

.product-image {
  max-width: 100%;
  height: auto;
}

.product-name {
  font-size: 1.2rem;
  margin: 8px 0;
  font-family: 'Norm' sans-serif;
  font-size: 18px;
  text-transform: uppercase;
  text-align: center;
  font-weight: 700;
  line-height: 21.6px;
  text-align: left;
}

.product-price {
  color: #666;
  font-family: 'Norm' sans-serif;
  font-size: 10px;
  font-weight: 400;
  line-height: 16.8px;
  text-align: center;
}
</style>
