<template>
  <div class="article-body">
    <div class="article-header">
      <h1>Founded in 1999 two friends, Terrance and Philip</h1>
    </div>
    <div class="article-content">
      <p> &ensp; What started as a hobby morphed into a world-class retailer where  collectors, enthusiasts, and first time owners are welcome. <br>
      &ensp; From insects to fishes and lizards, the ScalesEmporium has what you need and what you want!
      </p>
      <div class="article-image-container">
        <img src="../assets/images/fish1.jpg" alt="">
        <img src="../assets/images/fish1.jpg" alt="">
        <img src="../assets/images/fish1.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style>
.article-body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
}
.article-header {
  font-size: 2.5rem;
  text-decoration: underline;
}
.article-content {
  display: flex;
  justify-content: space-around;
  font-size: 1.5rem;
}
.article-image-container {
  width: 30vw;
}
.article-image-container img {
  border-radius: 50%;
  object-fit: contain;
  width: 50%;
}
@media (max-width: 800px) {
  .article-content {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .article-image-container img {
    width: 100%;
  }
}
</style>