<!-- src/components/Footer.vue -->

<template>
    <div class="app">
    <footer>
      <p>&copy; 2023 Department Business</p>
      <p>11 nhan trach, HanoiCity</p>
      <p>Email: nguynchikien1617@gmail.com</p>
  
      <!-- Liên kết mạng xã hội -->
      <div class="social-icons">
        <a href="#" target="_blank" title="Facebook"><i class="fab fa-facebook"></i></a>
        <a href="#" target="_blank" title="Twitter"><i class="fab fa-twitter"></i></a>
        <a href="#" target="_blank" title="Instagram"><i class="fab fa-instagram"></i></a>
      </div>
    </footer>
    </div>
  </template>
  
  <script>
  export default {
    name: 'FooterPage',
  };
  </script>
  
  <style scoped>
footer {
  background-color: #c7d4d9;
  color: #fff;
  padding: 20px;
  text-align: center;
}

footer p {
  margin: 5px 0;
}

/* Liên kết trong footer */
footer a {
  color: #fff;
  text-decoration: none;
}

/* Biểu tượng mạng xã hội */
.social-icons {
  margin-top: 10px;
}

.social-icons a {
  display: inline-block;
  margin: 0 10px;
  color: #fff;
  font-size: 20px;
}
</style>
  