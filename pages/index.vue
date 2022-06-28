<template>
  <div class="main" id="#main">
    <Navbar/>
    <Intro/>
    <Info/>
    <Gallery/>
    <Last/>
  </div>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,100;0,9..144,200;0,9..144,300;0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;0,9..144,800;0,9..144,900;1,9..144,100;1,9..144,200;1,9..144,300;1,9..144,400;1,9..144,500;1,9..144,600;1,9..144,700;1,9..144,800;1,9..144,900&family=Sen:wght@400;700;800&display=swap');
</style>


<script>
import { gsap } from "gsap";
import { ScrollTrigger } from '../js/ScrollTrigger.min.js';
gsap.registerPlugin(ScrollTrigger);

export default {
  name: 'IndexPage',
   mounted: function(){

    // INIZIO ANIMAZIONE NAVBAR
    gsap.to('#nav',{
      backgroundColor: '#0E0F12',
      scrollTrigger: {
      trigger: ".section-two",
        }
      });
    // FINE ANIMAZIONE NAVBAR

    gsap.to('.citazione', {opacity: 1, duration: 4, delay: 2}); // animazione sezione intro

    // INIZIO ANIMAZIONE SEZIONE INFO
    gsap.to('.tag_title',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 0.5,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-two",
        }
      });

    gsap.to('.flower_service',{ 
    opacity:1,
    duration: 1,
    delay: 0.5,
    scrollTrigger: {
      trigger: ".section-two",
        }
      });

    gsap.to('.our-services',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 1,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-two",
        }
    });

    gsap.to('.text-services',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 1.5,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-two",
        }
    });

    gsap.to('.read-services',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 2,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-two",
        }
    });

    // FINE ANIMAZIONE SEZIONE INFO

    // INIZIO ANIMAZIONE SEZIONE GALLERY

    gsap.to('.tag_title2',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 1.2,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-three",
        }
      });

    gsap.to('.new-entry',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 1.5,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-three",
        }
      });

    gsap.to('.section-carousel',{ 
      x:0,
      opacity:1,
      duration: 1.5,
      delay: 2,
      startAt: {x:300},
      scrollTrigger: {
        trigger: ".section-three",
          }
        });
    }
  }
</script>


