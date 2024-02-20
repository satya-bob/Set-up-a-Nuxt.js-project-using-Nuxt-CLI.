
import type productCard from './productCard.vue';

import type productCard from './productCard.vue';
<template>
    <div class="product-details">
      <div class="product-image-container">
        <img :src="product.image" alt="Product Image">
      </div>
      <div class="product-info">
        <h2>{{ product.title }}</h2>
        <h3>Price: ${{ product.price }}</h3>
        <h3>ID: {{ product.id }}</h3>
        <p>{{ product.description }}</p>
      </div>
    </div>
  </template>
  
  <script setup>
  const { product } = defineProps(["product"]);
  </script>
  
  <style scoped>
  .product-details {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .product-image-container {
    flex: 1;
    margin-right: 20px;
  }
  
  .product-info {
    flex: 2;
  }
  
  .product-image-container img {
    width: 100%;
    height: auto;
    border-radius: 5px;
    transition: transform 0.3s ease;
  }
  
  .product-image-container img:hover {
    transform: scale(1.05);
  }
  
  h2 {
    font-size: 24px;
    margin-bottom: 10px;
  }
  
  h3 {
    font-size: 20px;
    margin-bottom: 8px;
    color: #333;
  }
  
  p {
    font-size: 18px;
    color: #666;
  }
  </style>
  