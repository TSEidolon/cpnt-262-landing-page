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
.HeroContentContainer {
background-image: url("../assets/images/snake1.jpg");
height: 90vh;
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

.HeroText button {
background: "";
border: 1px solid #000000;
box-sizing: border-box;

box-shadow: 3px 6px 4px rgba(0, 0, 0, 0.25);
border-radius: 6px;
}


.HeroText img {
  width: 100%;
}

.HeroText p {
  color: white;
  font-size: 2rem;
  padding: 1rem;
}

.HeroText button {
  font-size: 1.7rem;
}

.HeroText button:hover {
  background-color: green;
}
</style>