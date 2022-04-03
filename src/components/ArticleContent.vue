<template>
  <div class="article-body">
    <div class="article-header">
      <h1>Founded in 1999 two friends, Terrance and Philip</h1>
    </div>
    <div class="article-content">
      <p> &ensp; What started as a hobby morphed into a world-class retailer where  collectors, enthusiasts, and first time owners are welcome. <br> <br>
      &ensp; Now with over 30 stores across Canada. From insects to fishes and lizards, the ScalesEmporium has what you need and what you want! 
      </p>
      <div class="article-image-container">
        <img src="../assets/images/fish1.jpg" alt="">
        <img src="../assets/images/fish1.jpg" alt="">
        <img src="../assets/images/fish1.jpg" alt="">
      </div>
    </div>
    <div class="custom-shape-divider-bottom-1648952350">
      <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
          <path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" opacity=".25" class="shape-fill"></path>
          <path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" opacity=".5" class="shape-fill"></path>
          <path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" class="shape-fill"></path>
      </svg>
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
  --quaternary-color: #173F3C; /* green 700*/
}

.article-body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  text-shadow: 3px 6px 4px rgba(0, 0, 0, 0.25);
  position: relative;

  background-color: var(--primary-color);
  color: var(--secondary-color);
}
.article-header {
  font-size: 2rem;
  /* text-decoration: underline; */
  margin-top: 3rem;
}
.article-content {
  display: flex;

  justify-content: space-around;
  align-items: stretch;
  font-size: 1.5rem;
  padding: 1rem;
  margin: 2rem 0;
  gap: 1rem;

}

.article-content p {
  width: 50%;
  text-align: start;
  margin-bottom: 3rem;
  
}


.article-image-container {
  width: 30vw;
  
}
.article-image-container img {
  border-radius: 50%;
  object-fit: contain;
  width: 50%;
}

/* SVG */
.custom-shape-divider-bottom-1648952350 {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}
.custom-shape-divider-bottom-1648952350 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 50px;
}
.custom-shape-divider-bottom-1648952350 .shape-fill {
    fill: #235F5A;
}

/* Media */
@media (max-width: 800px) {
  .article-content {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .article-image-container {
    margin-bottom: 2rem;
  }
  .article-image-container img {
    width: 100%;
  }
}
</style>