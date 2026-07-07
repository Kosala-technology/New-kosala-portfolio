.hero-image{

position:relative;

display:flex;

justify-content:center;

align-items:center;

}

/* Glow */

.hero-image::before{

content:"";

position:absolute;

width:420px;

height:420px;

background:radial-gradient(circle,
rgba(91,103,241,.25),
transparent 70%);

border-radius:50%;

z-index:-1;

animation:pulse 5s infinite;

}

.image-card{

width:390px;

height:500px;

padding:18px;

background:rgba(255,255,255,.65);

backdrop-filter:blur(20px);

border:1px solid rgba(255,255,255,.4);

border-radius:35px;

box-shadow:var(--shadow-lg);

animation:float 5s ease-in-out infinite;

}

@keyframes pulse{

0%,100%{

transform:scale(1);

opacity:.8;

}

50%{

transform:scale(1.08);

opacity:1;

}

}