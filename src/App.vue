<template>
  <div id="app">
    <header class="header">
      <div class="container">
        <h1 class="logo">SNEAKS HEAT</h1>
        <nav class="nav">
          <ul>
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/login">Login</router-link></li>
            <li><router-link to="/register">Register</router-link></li>
            <li><router-link to="/sneaker-list">Top Brands</router-link></li>
          </ul>
        </nav>
      </div>
    </header>

    <router-view></router-view>

    <footer class="footer">
      <div class="container">
        <p>&copy; Find the best sneakers of 2023</p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style scoped>


body {
    margin: 0;
    padding: 0;
    background: linear-gradient(to bottom, #0a032d, #0b30d5);
    color: navy;
    font-family: Arial, sans-serif;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }
  
  
  header {
    background-color: #30cfe7;
    color: #0f044f;
    padding: 10px 0;
  }
  
  header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  header h1 {
    color: #0a032d;
    font-size: 24px;
  }
  
  nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
  }
  
  nav li {
    font-size: 18px;
  }
  

  .hero {
    text-align: center;
    padding: 100px 0;
  }
  
  .hero h1 {
    font-size: 36px;
    margin-bottom: 20px;
  }
  
  .hero p {
    font-size: 18px;
    margin-bottom: 30px;
  }

  .featured-sneakers {
    padding: 40px 0;
    text-align: center;
  }
  
  .featured-sneakers h1 {
    font-size: 24px;
    margin-bottom: 20px;
  }
  

  @media (max-width: 768px) {
    header .container {
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
  
    header h1 {
      font-size: 20px;
      margin-bottom: 10px;
    }
  
    nav ul {
      flex-direction: column;
    }
  
    nav li {
      font-size: 16px;
    }
  
    .hero {
      padding: 60px 0;
    }
  
    .hero h1 {
      font-size: 28px;
    }
  
    .hero p {
      font-size: 16px;
    }
  
    .featured-sneakers h1 {
      font-size: 20px;
      margin-bottom: 15px;
    }
  }
  
</style>
