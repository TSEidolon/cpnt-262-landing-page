<template>
  <div class ="card-item-container">
    <div class="card-item-top">
      <img :src="props.src" class="card-item-image">
    </div>
    <div class="card-item-bottom">
      <h3 class="card-item-title"> {{props.title}}</h3>
      <p class="card-item-text">{{props.bgtext}}</p>
      <a href="#" target="_blank">
        <button class="card-item-button"> {{props.button}} &rarr; </button>
      </a>
    </div>
  </div>
</template>

<script setup>

import {defineProps} from 'vue';
  const props = defineProps({
  title: String,
  button: InputEvent,
  bgtext: String,
  src: Object,
})


  
</script>

<style >
:root {
  --primary-color:  #D5E5E4; /* green 100*/
  --secondary-color: #050D0C; /* green 900*/
  --tertiary-color:  #235F5A; /* green 600*/
}
  .card-item-container {
   display: flex;
   flex-direction: column;
   justify-content: center;
   align-items: center;
   /* padding: 1rem; */
   border-radius: 10px;
   background-color: var(--primary-color);
   box-shadow: 0 2rem 4rem rgba(0, 0, 0, 0.2);
   transition: all .5s ease-out;
   gap: 1rem;
}
.card-item-bottom {
  padding: 1rem;
  gap: 1rem;
}
.card-item-top {
  height: 80%;
}

.card-item-bottom a {
  text-decoration: none;
}
.card-item-container:hover {
  transform: translateY(-.5%);
  box-shadow: 0 3rem 6rem rgba(0, 0, 0, 0.4);
}

.card-item-image {
  object-fit: cover;
  width: 100%;
  height: 100%;
  border-top-left-radius: 10px ;
  border-top-right-radius: 10px ;
}
.card-item-text {
  font-size: 1.5rem;
  line-height: 1.2;
  color: var(--secondary-color);
  text-align: center;
  margin: 1rem;
  padding: 2rem 0;
}

.card-item-title {
  font-size: 2rem;
  color: var(--secondary-color);
  margin: 0;
}

.card-item-button {
  display: block;
  width: 100%;
  padding: 0.5rem;
  font-size: 1.8rem;
  text-align: center;
  background-color: var(--tertiary-color);
  color: var(--primary-color);
  border-radius: .5rem;
  transition: all .5s ease-out;
}

.card-item-button:hover {
  
  background-color: var(--secondary-color);
  color: var(--primary-color);
  word-spacing: 0.5rem;
  cursor: pointer;

}

</style>