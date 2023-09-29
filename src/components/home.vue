<template>
  <div>
    <header>
      <img
        src="https://img.freepik.com/premium-photo/sneakers-fire-burning-shoes-generative-aixa_174954-1847.jpg"
        width="50"
        height="50"
        alt="Sneakers Logo"
      />
    </header>

    <section class="hero">
      <div class="container">
        <h1>Welcome to SneakHeat</h1>
        <p>Discover the Best Sneakers</p>
      </div>
    </section>

    <section class="featured-sneakers">
      <div class="container">
        <h1>Featured Sneakers</h1>

        <div class="sneaker-wrapper">
          <a
            href="https://www.jd-sports.com.au/product/white-nike-dunk-low---1-per-customer/19582564_jdsportsau/"
            class="sneaker"
          >
            <img
              src="https://i8.amplience.net/i/jpl/jd_ANZ0054505_a?qlt=92&w=950&h=673&v=1&fmt=auto"
              alt="NIKE DUNKS"
            />
            <p>NIKE DUNKS</p>
          </a>
          <a
            href="https://www.jd-sports.com.au/product/red-jordan-air-5-retro-se---1-per-customer/19582458_jdsportsau/"
            class="sneaker"
          >
            <img
              src="https://i8.amplience.net/i/jpl/jd_669365_a?qlt=92&w=950&h=673&v=1&fmt=auto"
              alt="AIR JORDAN 5"
            />
            <p>AIR JORDAN 5</p>
          </a>
          <a
            href="https://www.jd-sports.com.au/product/adidas-originals-nmd-r1/19583753_jdsportsau/"
            class="sneaker"
          >
            <img
              src="https://i8.amplience.net/i/jpl/jd_GZ9256_C_0001_a?qlt=92&w=950&h=673&v=1&fmt=auto"
              alt="ADIDAS NMD"
            />
            <p>ADIDAS NMD</p>
          </a>
          <a
            href="https://www.jd-sports.com.au/product/green-new-balance-2002r/16213413_jdsportsau/"
            class="sneaker"
          >
            <img
              src="https://i8.amplience.net/i/jpl/jd_470326_a?qlt=92&w=950&h=673&v=1&fmt=auto"
              alt="NB 2002R"
            />
            <p>NB 2002R</p>
          </a>
        </div>
      </div>
    </section>

    <footer>
      <div class="container">
        <p>&copy; Find the best sneakers of 2023</p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {

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

.featured-sneakers {
  padding: 40px 0;
  text-align: center;
}

.featured-sneakers h1 {
  font-size: 24px;
  margin-bottom: 20px;
}

.sneaker-wrapper {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 20px;
}

.sneaker {
  text-decoration: none;
  color: #0a032d;
  background-color: #fff;
  border-radius: 5px;
  padding: 20px;
  text-align: center;
  width: calc(25% - 20px);
  transition: transform 0.2s ease-in-out;
}

.sneaker:hover {
  transform: scale(1.05);
}

.sneaker img {
  max-width: 100%;
}

.sneaker p {
  font-size: 18px;
  margin-top: 10px;
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

  .sneaker {
    width: calc(50% - 20px);
  }

  @media (max-width: 768px) {
  header .container {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }}
}

</style>
