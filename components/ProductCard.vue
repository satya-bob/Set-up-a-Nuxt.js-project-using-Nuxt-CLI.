
import type { ProductCard } from '#build/components';

import type { ProductCard } from '#build/components';

import type { ProductCard } from '#build/components';

  
  <template>
    <div class="product-item">
      <img :src="product.image" alt="Product Image">
      <NuxtLink :to="`/products/${product.id}`" class="details-link">View Details</NuxtLink>
    </div>
  </template>
  
  <script setup>
  const { product } = defineProps(['product']);
  </script>
  
  <style scoped>
  .product-item {
    position: relative;
    overflow: hidden;
  }
  
  .product-item img {
    width: 200px; /* Adjust the width to your preference */
    height: auto;
    transition: transform 0.3s ease;
  }
  
  .product-item:hover img {
    transform: scale(1.1);
  }
  
  .details-link {
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    background-color: #333;
    color: #fff;
    padding: 8px 16px;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s ease, transform 0.3s ease;
  }
  
  .details-link:hover {
    background-color: #555;
    transform: translate(-50%, -5px);
  }
  </style>
  