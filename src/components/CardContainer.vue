<template>
  <div class="card-container-body">
    <div class="products-area">
      <h1>Our Pets</h1>
    </div>
    <div class="card-container">
      <CardContainerContent 
      :title="products[0].title"
      :bgtext ="products[0].bgtext"
      :src ="products[0].src"
      :button ="products[0].button"  
      />
      <CardContainerContent 
      :title="products[0].title"
      :bgtext ="products[0].bgtext"
      :src ="products[0].src"
      :button ="products[0].button"  
      />
      <CardContainerContent 
      :title="products[0].title"
      :bgtext ="products[0].bgtext"
      :src ="products[0].src"
      :button ="products[0].button"  
      />
      <CardContainerContent 
      :title="products[0].title"
      :bgtext ="products[0].bgtext"
      :src ="products[0].src"
      :button ="products[0].button"  
      />
    </div>
    <div class="products-area-logo">
      <img src="../assets/svgs/LogoLight.svg" alt="Scales Emporium Logo Light">
    </div>
  </div>
</template>

<script setup>
import CardContainerContent from './CardContainerContent.vue';

const products = ([
        {
          title: 'Forest One',
          button: 'More',
          bgtext: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magnam pariatur.',
          src: require('../assets/images/fish1.jpg'),
        },
        {
          title: 'Forest Two',
          button: 'More',
          bgtext: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magnam pariatur.',
          src: require('../assets/images/fish1.jpg'),
        },
        {
          title: 'Forest Three',
          button: 'More',
          bgtext: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magnam pariatur.',
          src: require('../assets/images/fish1.jpg'),
        }
])
</script>

<style>
.card-container-body {
  display:flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
  text-align: center;
  padding: 1rem;
  gap: 1rem;
}
 .card-container {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
gap: 1.5rem;
border: 1rem;
}

.products-area-logo {
width: 70px;
margin-top: 1rem;
}
</style>