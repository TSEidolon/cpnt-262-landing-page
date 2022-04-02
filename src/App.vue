<template>
  <div>
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->

      <TheNav />

      <HeroContent />

      <CardContainer />

      <ArticleContent />

      <TheFooter />

  </div>
  
</template>

<script setup> // setup === important
  import TheNav from './components/TheNav.vue';
  import HeroContent from './components/HeroContent.vue';
  import CardContainer from './components/CardContainer.vue';
  import ArticleContent from './components/ArticleContent.vue';
  import TheFooter from './components/TheFooter.vue'
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=PT+Sans+Narrow&display=swap');

#app {
  font-family: 'PT Sans Narrow', sans-serif;

}

/* Resets */
*, *::before, *::after {
  box-sizing: border-box;
}

* {
  margin: 0;
}

html, body {
  height: 100%;
}
/*  */
</style>
