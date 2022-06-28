<!-- Please remove this file from your project -->
<template>
  <section class="section section-one">
    <div class="container">
      <div class="introduzione">
        <div class="animation">
          <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
          <lottie-player src="https://assets4.lottiefiles.com/private_files/lf30_IeIbXu.json"  background="transparent"  speed="1"  style="width: 170px; height: 170px;"  loop  autoplay></lottie-player>
        </div>
        <p class="citazione">"A flower’s appeal is in its contradictions so delicate in form yet strong in fragrance, so small in size yet big in beauty, so short in life yet long on effect."</p>
        <div class="animation">
          <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
          <lottie-player src="https://assets4.lottiefiles.com/private_files/lf30_IeIbXu.json"  background="transparent"  speed="1"  style="width: 170px; height: 170px;"  loop  autoplay></lottie-player>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
  section {
    height: 100vh;
  }

 .section-one {
   background-image: url('../img/Background.png');
   background-size: cover;
   background-repeat: no-repeat;
   height: 100vh;
 }

 .container {
   position: relative;
   top: 150px;
   margin: 0 auto;
   padding: 0;
 }

 .citazione {
   color: white;
   text-align: center;
   font-family: 'Fraunces', serif;
   font-size: 1.8rem;
   opacity: 0;
 }

 .animation {
   display: flex;
   justify-content: center;
   z-index: 998;
   transform: rotate(-45deg);
 }

  @media (max-width: 768px){
    .citazione {
      color: white;
      text-align: center;
      font-family: 'Fraunces', serif;
      font-size: 1.2rem;
      opacity: 0;
    }
  }


</style>

<script>
export default {
  name: 'Intro'
}
</script>
