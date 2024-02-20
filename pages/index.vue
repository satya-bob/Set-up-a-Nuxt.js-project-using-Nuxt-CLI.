<template>
  <div class="home-page">
    <h1>Welcome to Our Website!</h1>
    <p>This is the home page of our website.</p>
    
    
  </div>
</template>

<script setup>

</script>
<style>
.home-page {
  text-align: center;
}
/* Styles for the heading */
h1 {
  font-size: 36px;
  color: #333;
}

/* Styles for the paragraph */
p {
  font-size: 18px;
  color: #666;
}

/* Hover effect for the heading */
h1:hover {
  color: #ff9900;
  cursor: pointer;
  transition: color 0.3s ease;
}

/* Hover effect for the paragraph */
p:hover {
  color: #4caf50;
  cursor: pointer;
  transition: color 0.3s ease;
}

/* Animation for the heading */
@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-30px);
  }
  60% {
    transform: translateY(-15px);
  }
}


</style>
