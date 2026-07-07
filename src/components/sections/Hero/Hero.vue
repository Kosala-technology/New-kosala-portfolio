<template>
  <section id="home" class="hero">

    <HeroBackground />

    <div class="container hero-container">

      <HeroContent />

      <HeroImage />

    </div>

  </section>
</template>

<script setup>
import HeroContent from "./HeroContent.vue";
import HeroImage from "./HeroImage.vue";
import HeroBackground from "./HeroBackground.vue";
</script>

<style scoped>

.hero{

    min-height:100vh;

    position:relative;

    overflow:hidden;

    display:flex;

    align-items:center;

    padding-top:120px;

}

.hero-container{

    position:relative;

    z-index:2;

    display:grid;

    grid-template-columns:1.1fr .9fr;

    gap:80px;

    align-items:center;

}

@media(max-width:992px){

.hero-container{

grid-template-columns:1fr;

}

}

</style>