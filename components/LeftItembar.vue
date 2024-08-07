<template>
  <div class="container">
    <div class="checkbox">
      <input id="Customizble" type="checkbox" />
      <label for="Customizble">Customizble</label>
    </div>
    <div class="dropdown">
      <AccordionDropdown :items="accordionItems" />
      <ProductGrid :products="products" />
    </div>
  </div>
</template>
<script>
import AccordionDropdown from './AccordionDropdown.vue'
import ProductGrid from './ProductGrid.vue'

export default {
  components: {
    AccordionDropdown,
    ProductGrid,
  },
  data() {
    return {
      isOpen: false,
      options: ['Option 1', 'Option 2', 'Option 3'],
      selectedOptions: [],

      accordionItems: [
        {
          title: 'IDEAL FOR',
          content: 'This is the content of item 1.',
        },
        {
          title: 'OCCASION',
          content: 'This is the content of item 2.',
        },
        {
          title: 'WORK',
          content: 'This is the content of item 3.',
        },
        {
          title: 'FABRIC',
          content: 'This is the content of item 4.',
        },
        {
          title: 'SEGMENT',
          content: 'This is the content of item 5.',
        },
        {
          title: 'RAW MATERIAL',
          content: 'This is the content of item 6.',
        },
        {
          title: 'PATTERN',
          content: 'This is the content of item 3.',
        },
      ],
      products: [
        {
          id: 1,
          name: 'PPXOC Milkyway dress in pressed flowers',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/Product_Image.png',
        },
        {
          id: 2,
          name: 'PPXOC Milkyway dress in pressed flowers',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/Rectangle 29438.png',
        },
        {
          id: 3,
          name: 'Product Name',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/Rectangle 29438product-2.png',
        },
        {
          id: 4,
          name: 'Product Name',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/product-4.png',
        },
        {
          id: 5,
          name: 'Product Name',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/product-3.png',
        },
        {
          id: 6,
          name: 'Product Name',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/product-4.png',
        },
        {
          id: 7,
          name: 'Product Name',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/product-4.png',
        },
        {
          id: 8,
          name: 'Product Name',
          content: 'Sign in or Create an account to see pricing',
          image: '/assets/Product_Image.png',
        },
      ],
    }
  },
}
</script>
<style scoped>
.checkbox {
  border-bottom: 1px solid;
}
.dropdown {
  display: flex;
  padding: 5%;
  /* align-items: center; */
  gap: 10%;
  justify-content: space-between;
  width: 100%;
}

.dropdown-button {
  /* background-color: #4caf50; */
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

.dropdown-menu {
  display: block;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
  padding: 12px 16px;
}

.dropdown-item {
  padding: 12px 16px;
  cursor: pointer;
}

.dropdown-item label {
  display: flex;
  align-items: center;
}

.dropdown-item input[type='checkbox'] {
  margin-right: 8px;
}
</style>
