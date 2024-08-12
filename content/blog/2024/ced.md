---
title: "Creative Engineering Design"
author: "Abhijeet"
weight: 1
date: 2024-08-12
lastmod: 2024-08-12
dateString: August 2024 
description: "Creative Engineering Design"
#canonicalURL: "https://canonical.url/to/page"
cover:
    image: ".VedMobile.png" # image path/url
    alt: "Download Logo" # alt text
    #caption: "Optical Character Recognition"  display caption under cover 

tags: [ "Design", "codefrydev", "UI/UX", "CFD", "user interface","user exprience","app design", "Card Shorting", "Research", "Creative Engineering Design", "CED"]
keywords: ["Design", "codefrydev", "UI/UX", "CFD", "user interface","user exprience","app design","Ved Mobile","app","FFMPEG", "Creative Engineering Design", "CED"]

---

<style>

@import url('https://fonts.googleapis.com/css2?family=Rubik+Mono+One&display=swap');

    :root {
  --font_family_for_threeD: "Rubik Mono One", monospace;
  --color_for_texture: #ffffff; 
}


@media (orientation: landscape) {
  main {
    scale: 0.9;
  }
}


 
main {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  perspective: 1000px;
}

#threeD_section {
  aspect-ratio: 9/14;
  background: center/cover no-repeat url("./bg.png");
  width: 100%;
  max-width: 70vmin;
  position: relative;
  animation: move 100s 0s infinite;
  transform-style: preserve-3d;
  border-radius: 6vmin;
}

#main_hero_text_texture {
  position: absolute;
  top: 30%;
  left: 0;
  width: 100%;
  text-align: center;
  display: flex;
  justify-content: center;
  transform: translateZ(10vmin);
  transform-style: preserve-3d;
}

#main_hero_text {
  font-family: var(--font_family_for_threeD);
  font-size: 22vmin;
  position: absolute;
  margin: 0;
  line-height: 1em;
  white-space: nowrap;
  background-image: url("./texture.png");
  background-size: cover;
  background-position: center;
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
}

#main_hero_text::before {
  content: attr(data-title);
  position: absolute;
  color:  var(--color_for_texture);
  -webkit-text-fill-color: initial;
  mix-blend-mode: overlay;
  opacity: 1;
  text-shadow: 0px 0px 4vmin rgba(0, 0, 0, 0.4), 1px 1px  var(--color_for_texture);
}

#front_image_threeD_poster {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: auto;
  transform: translateZ(20vmin);
  transform-style: preserve-3d;
  filter: drop-shadow(0px 0px 40px rgba(0, 0, 0, 0.4));
  border-radius: 6vmin;
}

#first_author_wother_name {
  font-family: var(--font_family_for_threeD);
  font-size: 2.6vmin;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--color_for_texture);
  text-shadow: 0px 0px 3vmin rgba(0, 0, 0, 0.7);
  position: absolute;
  top: 5%;
  left: 6%;
  transform: translateZ(5vmin);
  transform-style: preserve-3d;
  margin: 0;
}

#author_wother_name {
  font-family: var(--font_family_for_threeD);
  font-size: 2.6vmin;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--color_for_texture);
  text-shadow: 0px 0px 3vmin rgba(0, 0, 0, 0.7);
  position: absolute;
  top: 5%;
  right: 6%;
  transform: translateZ(5vmin);
  transform-style: preserve-3d;
  margin: 0;
}

#top_long_text {
  font-family: var(--font_family_for_threeD);
  font-size: 3vmin;
  text-transform: uppercase;
  text-align: center;
  color: white;
  letter-spacing: 0.4em;
  width: 100%;
  position: absolute;
  top: 26%;
  left: 0%;
  transform: translateZ(5vmin);
  transform-style: preserve-3d;
  margin: 0;
}

#top_long_text strong {
  font-family: var(--font_family_for_threeD);
}

#middle_big_title_text {
  display: flex;
  justify-content: space-between;
  font-family: var(--font_family_for_threeD);
  font-size: 5vmin;
  line-height: 1em;
  text-align: center;
  white-space: nowrap;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  position: absolute;
  top: 48%;
  left: 0%;
  width: 100%;
  margin: 0;
  transform: translateZ(10vmin);
  /* transform-style: preserve-3d; */
  /* text-shadow: 0px 0px 4vmin rgba(0,0,0,0.4); */
}

#middle_big_title_text > span {
  display: flex;
  background-image: url("./texture.png");
  background-size: cover;
  background-position: center;
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
}

#middle_big_title_text > span::before {
  content: attr(data-title);
  position: absolute;
  color:  var(--color_for_texture);
  -webkit-text-fill-color: initial;
  mix-blend-mode: overlay;
  opacity: 1;
  text-shadow: 0px 0px 4vmin rgba(0, 0, 0, 0.4), 1px 1px  var(--color_for_texture);
}

#main_hero_text {
    pointer-events: none; /* disables all pointer events, including hover */
}

/*for fixed animation*/

 /* .animated-element {
            
            transition: transform 0.2s ease;
            transform-style: preserve-3d;
        }
        .container:hover .animated-element {
            transform: rotateX(-10deg) rotateY(10deg);
        } */
/*for auto rotating*/
        /* @keyframes move {
  0% {
    transform: rotateY(-20deg) rotateX(-5deg);
  }
  25% {
    transform: rotateY(20deg) rotateX(-5deg);
  }
  50% {
    transform: rotateY(20deg) rotateX(5deg);
  }
  75% {
    transform: rotateY(-20deg) rotateX(5deg);
  }
  100% {
    transform: rotateY(-20deg) rotateX(-5deg);
  }
} */

 @keyframes move {
  0% {
    transform: rotateY(-20deg) rotateX(-5deg);
  }
  10% {
    transform: rotateY(30deg) rotateX(10deg);
  }
  20% {
    transform: rotateY(-10deg) rotateX(-20deg);
  }
  30% {
    transform: rotateY(25deg) rotateX(15deg);
  }
  40% {
    transform: rotateY(-15deg) rotateX(-25deg);
  }
  50% {
    transform: rotateY(20deg) rotateX(20deg);
  }
  60% {
    transform: rotateY(-25deg) rotateX(-10deg);
  }
  70% {
    transform: rotateY(10deg) rotateX(30deg);
  }
  80% {
    transform: rotateY(-30deg) rotateX(5deg);
  }
  90% {
    transform: rotateY(5deg) rotateX(-15deg);
  }
  100% {
    transform: rotateY(-20deg) rotateX(-5deg);
  }
}


</style>

<main class="container">
    <article id="threeD_section" class="animated-element" >
        <header id="main_hero_text_texture" >
            <h1 id="main_hero_text" data-title="TINY">TINY</h1>
        </header>
        <p id="first_author_wother_name">FREEDOM SALE</p>
        <p id="author_wother_name">100% OFF</p>
        <p id="top_long_text">CODE FRY DEV<strong></strong></p>
        <p id="middle_big_title_text">
            <span data-title="ARCADE">ARCADE</span> 
            <span data-title="GAME">GAME</span>
        </p>
        <img id="front_image_threeD_poster" src="./front.png"  alt="Furiosa Front image">
    </article>
</main>
