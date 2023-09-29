<template>
  <div>
    <h2>Sneakers Brands</h2>
    <ul>
      <li v-for="sneaker in sneakers" :key="sneaker.id">

        <a :href="sneaker.brandWebsite" target="_blank">
          <img :src="sneaker.brandLogo" alt="Brand Logo" width="100" />
        </a>
        <button @click="openBrandWebsite(sneaker.brandWebsite)">Visit Website</button>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sneakers: [
        {
          id: 1,
          brand: 'Nike',
          brandWebsite: 'https://www.nike.com/au/',
          brandLogo: 'https://w0.peakpx.com/wallpaper/909/798/HD-wallpaper-nike-nike-logo-smoke-nike-sunset-brand-iphone.jpg',
        },
        {
          id: 2,
          brand: 'Adidas',
          brandWebsite: 'https://www.adidas.com.au/?cm_mmc=AdieSEM_Google-_-PPC-B-Brand-Other-AU-SEAPAC-eCom-Paid_Search-_-Brand-X-X-General-_-adidas-_-dv:eCom&cm_mmc1=AU&cm_mmc2=e&gclid=CjwKCAjwu4WoBhBkEiwAojNdXllUD3XrzXrw9Pez1n485qtDCMwvwDLQgKHsJyRXrXQDqklkEAQvCRoCr2EQAvD_BwE&gclsrc=aw.ds',
          brandLogo: 'https://i.pinimg.com/236x/fe/33/a5/fe33a5eb70cf15be030bc5ab5b308e7c.jpg',
        },
        {
          id: 3,
          brand: 'Jordan',
          brandWebsite: 'https://www.nike.com/au/jordan',
          brandLogo: 'https://i.etsystatic.com/36071809/r/il/c40a8a/3977487189/il_570xN.3977487189_eiyn.jpg',
        },
        {
          id: 4,
          brand: 'New Balance',
          brandWebsite: 'https://www.newbalance.com.au',
          brandLogo: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQIXd73rMmtKDG4zDG9dWECswUGL-oGnEVQ1u7O5-dinnfylFM8P6Fw5FH1wwq7jR61IH8&usqp=CAU',
        },
      ],
    };
  },
  methods: {
    openBrandWebsite(brandWebsite) {
      window.open(brandWebsite, '_blank');
    },
  },
};
</script>
<style scoped>

.brand-logo {
  width: 100px; 
  height: 100px; 
}


body {
  margin: 0;
  padding: 0;
  background: linear-gradient(to bottom, #0a032d, #0b30d5);
  color: navy;
  font-family: Arial, sans-serif;
}
</style>