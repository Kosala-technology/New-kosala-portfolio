<template>

<div class="hero-content">

    <span class="welcome">
        👋 Welcome to my portfolio
    </span>

    <h1>

        Kosala Lakshan

        <span>Samararathna</span>

    </h1>

    <h2 id="typing">
        Software Engineering Intern
    </h2>

    <p>

        I build modern, responsive and user-focused web applications with clean code and beautiful user experiences.

    </p>

    <div class="buttons">

        <a href="#" class="btn">
            Download CV
        </a>

        <a href="#contact" class="btn secondary">

            Contact Me

        </a>

    </div>

</div>

</template>

<script setup>

</script>

<style scoped>

.hero-content{

display:flex;

flex-direction:column;

gap:25px;

}

.welcome{

display:inline-flex;

align-items:center;

width:max-content;

padding:10px 20px;

border-radius:999px;

background:white;

box-shadow:var(--shadow-sm);

font-size:.9rem;

}

h1{

font-size:68px;

line-height:1.05;

font-weight:700;

}

h1 span{

display:block;

color:var(--primary-color);

}

h2{

font-size:26px;

color:var(--text-secondary);

font-weight:500;

}

p{

font-size:18px;

max-width:620px;

color:var(--text-secondary);

}

.buttons{

display:flex;

gap:20px;

margin-top:10px;

}

.secondary{

background:white;

color:var(--text-primary);

border:1px solid var(--border-color);

}

.secondary:hover{

background:var(--primary-color);

color:white;

}

@media(max-width:992px){

.welcome{

margin:auto;

}

.buttons{

justify-content:center;

}

h1{

font-size:50px;

}

}

</style>

<script setup>
import { ref, onMounted, onBeforeUnmount } from "vue";
import Typed from "typed.js";

const typingElement = ref(null);

let typed;

onMounted(() => {

  typed = new Typed(typingElement.value, {

    strings: [

      "Software Engineering Intern",

      "Frontend Developer",

      "Vue.js Developer",

      "UI Enthusiast",

      "Problem Solver"

    ],

    typeSpeed: 60,

    backSpeed: 40,

    backDelay: 1800,

    loop: true

  });

});

onBeforeUnmount(() => {

  typed.destroy();

});
</script>