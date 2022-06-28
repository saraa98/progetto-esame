<!-- Please remove this file from your project -->
<template>
  <section class="section section-correlate">
    <div class="animation animation-rose">
      <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
      <lottie-player src="https://assets4.lottiefiles.com/private_files/lf30_IeIbXu.json"  background="transparent"  speed="1"  style="width: 170px; height: 170px;"  loop  autoplay></lottie-player>
    </div>
    <h3 class="title_correlati">More for you</h3>
    <div class="img-correlate">
      <div class="fiore-correlato correlato1">
        <img src="../img/prime.jpg" />
        <span><h3><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
          <line y1="1" x2="106" y2="1" stroke="white" stroke-width="1.5"/> </svg>Lotus Flower</h3></span>
      </div>
      <div class="fiore-correlato correlato2">
      <img src="../img/violet.jpg" />
      <span><h3><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
                <line y1="1" x2="106" y2="1" stroke="white" stroke-width="1.5"/> </svg>Primrose</h3></span>
      </div>
      <div class="fiore-correlato correlato3">
      <img src="../img/flower3.jpg" />
      <span><h3><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
                <line y1="1" x2="106" y2="1" stroke="white" stroke-width="1.5"/> </svg>Lotus Flower</h3></span>
      </div>
    </div>
  </section>
</template>

<style>
  .section-correlate {
    background-color: #0E0F12;
    height: 85vh;
  }

  .section-correlate .animation {
    z-index: 0 !important;
  }

  .title_correlati {
    text-align: center;
    font-family: 'Fraunces', serif;
    font-size: 2.5rem;
    font-style: italic;
    font-weight: 600;
    color: #8B9EFF;
    margin-top: 0;
    opacity: 0;
  }

  .img-correlate {
    display: flex;
    justify-content: space-evenly;
    position: relative;
    top: 30px;
    z-index: 998;
    opacity: 0;
  }

  .img-correlate img {
    width: 380px;
    height: 256px;
    transition: 0.6s;
  }

  .fiore-correlato span h3 {
    color: white;
    font-family: 'Fraunces', serif;
    font-size: 1.8rem;
    font-style: italic;
    font-weight: 400;
    text-align: center;
    text-shadow: 2px 2px black;
    margin-top: 15px;
    opacity: 0;
    position: relative;
    top: -160px;
    z-index: 998;
    transition: 0.6s;
  }

  .fiore-correlato:hover span h3 {
    opacity: 1;
  }

  .fiore-correlato:hover img {
    filter: blur(1px);
    border-radius: 32px;
    border: 0.2px solid white;
  }

  @media (max-width: 768px) {
    .section-correlate {
      background-color: #0E0F12;
      height: 145vh;
    }

    .title_correlati {
      text-align: center;
      font-family: 'Fraunces', serif;
      font-size: 2rem;
      font-style: italic;
      font-weight: 600;
      color: #8B9EFF;
      margin-top: 0;
      opacity: 0;
    }

    .img-correlate {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    position: relative;
    top: 30px;
    z-index: 998;
    opacity: 0;
  }
  .img-correlate img {
    width: 280px;
    height: 188px;
    transition: 0.6s;
  }

  .fiore-correlato span h3 {
    color: white;
    font-family: 'Fraunces', serif;
    font-size: 1.5rem;
    font-style: italic;
    font-weight: 400;
    text-align: center;
    text-shadow: 2px 2px black;
    margin-top: 15px;
    opacity: 0;
    position: relative;
    top: -125px;
    z-index: 998;
    transition: 0.6s;
  }

  }

</style>
 
<script>
export default {
  name: 'Correlati'
}
</script>
