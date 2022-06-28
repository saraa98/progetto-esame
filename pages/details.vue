<template>
   <div>
    <Navbar/>
    <InfoDettaglio/>
    <Correlati/>
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
      trigger: ".section-details",
        }
      });
    // FINE ANIMAZIONE NAVBAR

    // INIZIO ANIMAZIONE SECTION DETAILS
    gsap.to('.img_details', {opacity: 1, duration: 3, delay: 1.2});

    gsap.to('.tag-img-rose',{ 
    x:0,
    opacity:1,
    duration: 2,
    delay: 1.2,
    startAt: {x:-100},
    scrollTrigger: {
      trigger: ".section-details",
        }
      });

    gsap.to('.title-img-rose',{ 
    x:0,
    opacity:1,
    duration: 2,
    delay: 1.5,
    startAt: {x:-100},
    scrollTrigger: {
      trigger: ".section-details",
        }
      });

    gsap.to('.text-img-rose',{ 
    y:0,
    opacity:1,
    duration: 1.5,
    delay: 2,
    startAt: {y:100},
    scrollTrigger: {
      trigger: ".section-details",
        }
      });
    
    gsap.to('.order',{ 
    y:0,
    opacity:1,
    duration: 1.7,
    delay: 2.2,
    startAt: {y:100},
    scrollTrigger: {
      trigger: ".section-details",
        }
      });

    gsap.to('.elenco-descrizione',{ 
    y:0,
    opacity:1,
    duration: 1.7,
    delay: 2.4,
    startAt: {y:100},
    scrollTrigger: {
      trigger: ".section-details",
        }
      });
    
    // FINE ANIMAZIONE SECTION DETAILS

    // INIZIO ANIMAZIONE SECTION CORRELATI
    
    gsap.to('.title_correlati',{ 
    y:0,
    opacity:1,
    duration: 1.5,
    delay: 4.5,
    startAt: {y:-60},
    scrollTrigger: {
      trigger: ".section-correlate",
        }
      });

    gsap.to('.img-correlate',{ 
    y:0,
    opacity:1,
    duration: 1.5,
    delay: 4.5,
    startAt: {y:100},
    scrollTrigger: {
      trigger: ".section-correlate",
        }
      });
    
  }
}
</script>
