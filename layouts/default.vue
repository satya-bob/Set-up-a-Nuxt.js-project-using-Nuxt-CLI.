<template>
    <div>
      <header class="header">
        <nav class="nav">
          <NuxtLink to="/" class="nav-link">Satya Website</NuxtLink>
        </nav>
      </header>
      <div class="content">
        <slot />
      </div>
      <footer class="footer">
        <ul class="footer-links">
          <li><NuxtLink to="/" class="footer-link">Home</NuxtLink></li>
          <li><NuxtLink to="/about" class="footer-link">About</NuxtLink></li>
          <li><NuxtLink to="/products" class="footer-link">Products</NuxtLink></li>
        </ul>
      </footer>
    </div>
  </template>
  
  <style scoped>
  .header {
    background-color: #333;
    color: #fff;
    padding: 20px;
  }
  
  .nav {
    display: flex;
    justify-content: space-between;
  }
  
  .nav-link {
    color: #fff;
    font-weight: bold;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  .nav-link:hover {
    color: #ff6600;
  }
  
  .content {
    padding: 20px;
  }
  
  .footer {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
  }
  
  .footer-links {
    list-style-type: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
  }
  
  .footer-link {
    color: #fff;
    text-decoration: none;
    margin: 0 10px;
    transition: color 0.3s ease;
  }
  
  .footer-link:hover {
    color: #ff6600;
  }
  </style>
  