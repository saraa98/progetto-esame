<template>
  <div>
    <Navbar/>
    <Aboutintro/>
    <AboutInfo/>
    <Awards/>
    <Last/>
  </div>
</template>

<style>
  .home-enter-active, .home-leave-active {transition: opacity 0.5s; }
  .home-enter, .home-leave-active { opacity: 0; }
</style>



<script>
import { gsap } from "gsap";
import { ScrollTrigger } from '../js/ScrollTrigger.min.js';
gsap.registerPlugin(ScrollTrigger);

export default {
  name: 'IndexPage',
  transition: 'home',
  mounted: function(){

    // INIZIO ANIMAZIONE NAVBAR
    gsap.to('#nav',{
      backgroundColor: '#0E0F12',
      scrollTrigger: {
      trigger: ".section-about-info",
        }
      });

    // FINE ANIMAZIONE NAVBAR

    gsap.to('.about-intro', {opacity: 1, duration: 2, delay: 1.2}); // ANIMAZIONE SEZIONE ABOUT INTRO

    //INIZIO ANIMAZIONE SEZIONE ABOUT INFO
    gsap.to('.title-spiegazione',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 1.2,
    startAt: {x:-80},
    scrollTrigger: {
      trigger: ".section-about-info",
        }
      });
    
    gsap.to('.paragrafo',{ 
    x:0,
    opacity:1,
    duration: 1,
    delay: 1.2,
    startAt: {x:380},
    scrollTrigger: {
      trigger: ".section-about-info",
        }
      });

    //FINE ANIMAZIONE SEZIONE ABOUT INFO

    //INIZIO ANIMAZIONE SEZIONE AWARDS

    gsap.to('.row-awards',{ 
    y:0,
    opacity:1,
    duration: 2,
    delay: 1.5,
    startAt: {y:150},
    scrollTrigger: {
      trigger: ".section-about-awards",
        }
      });

    gsap.to('.hr',{ 
    opacity:1,
    duration: 2,
    delay: 1.5,
    scrollTrigger: {
      trigger: ".section-about-awards",
        }
      });

    //FINE ANIMAZIONE SEZIONE AWARDS

  }
}
</script>
