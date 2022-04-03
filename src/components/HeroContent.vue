<template>
  <div>
    <div class="HeroContentContainer">
      <div class="HeroText">
          <img src="../assets/svgs/HeroLogoLight.svg" alt="Scales Emporium Logo Light">
          <p> Your one stop shop for all your scaly friends</p>
          <button> Shop Now! </button>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style>
:root {
  --primary-color:  #D5E5E4; /* green 100*/
  --secondary-color: #050D0C; /* green 900*/
  --tertiary-color:  #235F5A; /* green 600*/
  --quarternary-color: #173F3C; /* green 700*/
}

.HeroContentContainer {
background-image: url("../assets/images/snake1.jpg");
height: 95vh; /* */
background-size: cover;
background-repeat: no-repeat;

display: flex;
justify-content: start;
align-items: center;
text-align: center;
width: 100%;
}
.HeroText {
  margin-left: 20%;
  width: 25%;
}

@media (max-width: 800px) {
  .HeroText {
    width: 70%;
    margin: 10%;
    padding: 10%;
  }
}

.HeroText button {
background-color: var(--tertiary-color);
color: var(--primary-color);
border: 1px solid black;
box-sizing: border-box;

box-shadow: 3px 6px 4px rgba(0, 0, 0, 0.25);
border-radius: 6px;
padding: 5px 20px;
font-size: 1.7rem;
}


.HeroText img {
  width: 100%;
}

.HeroText p {
  color: white;
  font-size: 2rem;
  padding: 1rem;
  text-shadow: 2px 2px black;
  transition: all 2s ease-out;
}



.HeroText button:hover {
  transform: translateY(-5%);
  background-color: var(--primary-color);
  color: var(--secondary-color);
  box-shadow: 3px 6px 4px rgba(0, 0, 0, 0.4);
  cursor: pointer;
}
</style>