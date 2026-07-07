<template>

<div class="experience-card">

    <h3>💼 Experience</h3>

    <p>Software Engineering Intern</p>

</div>

</template>

<script setup>

</script>

<style scoped>

.experience-card{

position:absolute;

left:-30px;

bottom:40px;

background:white;

padding:20px;

border-radius:20px;

box-shadow:var(--shadow-md);

width:220px;

}

h3{

margin-bottom:8px;

}

p{

color:var(--text-secondary);

}

@media(max-width:992px){

.experience-card{

position:relative;

left:0;

bottom:0;

margin-top:20px;

width:100%;

}

}

</style>