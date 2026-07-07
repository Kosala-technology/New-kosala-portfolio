<template>

<div class="background">

    <div class="blob blob1"></div>

    <div class="blob blob2"></div>

    <div class="blob blob3"></div>

    <div class="grid"></div>

</div>

</template>

<script setup>

</script>

<style scoped>

.background{

position:absolute;

inset:0;

overflow:hidden;

z-index:0;

}

/* Background Grid */

.grid{

position:absolute;

inset:0;

background-image:

linear-gradient(rgba(0,0,0,.04) 1px, transparent 1px),

linear-gradient(90deg, rgba(0,0,0,.04) 1px, transparent 1px);

background-size:40px 40px;

opacity:.4;

}

/* Blobs */

.blob{

position:absolute;

border-radius:50%;

filter:blur(80px);

animation:move 12s ease-in-out infinite;

}

.blob1{

width:350px;

height:350px;

background:#7C83FD;

top:-120px;

left:-100px;

opacity:.35;

}

.blob2{

width:300px;

height:300px;

background:#63B3ED;

right:-80px;

top:180px;

opacity:.3;

animation-delay:2s;

}

.blob3{

width:250px;

height:250px;

background:#B794F4;

bottom:-80px;

left:45%;

opacity:.25;

animation-delay:4s;

}

@keyframes move{

0%{

transform:translate(0,0);

}

50%{

transform:translate(40px,-30px);

}

100%{

transform:translate(0,0);

}

}

</style>