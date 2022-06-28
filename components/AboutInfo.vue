<!-- Please remove this file from your project -->
<template>
  <section class="section section-about-info">
    <div class="spiegazione">
      <div class="title-spiegazione">
        <h2>Our Story</h2>
          <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
          <lottie-player class="animation" src="https://assets4.lottiefiles.com/private_files/lf30_IeIbXu.json"  background="transparent"  speed="1"  style="width: 170px; height: 170px;"  loop  autoplay></lottie-player>
      </div>
      <div class="paragrafo col col-8">
        <p class="text-spiegazione"> The brand was born of a desire to bring the finest florals from across the globe, to our country. Working with floral design and installations across Europe, made us long to carry home some of the natural beauty we witnessed, to bring an elevated new look to our own weddings and special occasions. These exquisite natural flowers are now available in India, ordered with ease and delivered with transparency, to challenge the boundaries of all our celebrations could be.</p>
      </div>
    </div>
  </section>
</template>

<style>

  .section-about-info {
    background-color: #0E0F12;
    height: 65vh;
  }
  .spiegazione {
    display: flex;
    justify-content: center;
    position: relative;
    top: 45px;
    margin-left: 100px;
    margin-right: 100px;
    padding-top: 20px;
  }

  .title-spiegazione {
    margin-right: 200px;
    padding-left: 100px;
    position: relative;
    left: 100px;
    top: 20px;
    opacity: 0;
  }

  .title-spiegazione h2{
    font-family: 'Fraunces', serif;
    font-size: 2.5rem;
    font-weight: 600;
    color: #8B9EFF;
    margin-bottom: 0;
  }

  .paragrafo {
    padding-left: 100px;
    padding-right: 60px;
    opacity: 0;
  }

  .text-spiegazione {
    color:white;
    font-family: 'Sen', sans-serif;
    font-size: 1.2rem;
    line-height: 34px;
    margin-top: 10px;

  }
@media (max-width: 768px){
  .section-about-info{
    background-color: #0E0F12;
    height: 105vh;
  }
  .spiegazione {
    position: relative;
    top: 5px;
    padding-top: 10px;
    margin: 0 auto;
  }
  .title-spiegazione {
    position: relative;
    left: 200px;
    opacity: 0;
  }
  .title-spiegazione h2{
    padding-left: 15px;
    font-family: 'Fraunces', serif;
    font-size: 2rem;
    font-weight: 600;
    color: #8B9EFF;
    margin-bottom: 0;
    position: relative;
    top: 200px;
  }
  .paragrafo {
    position: relative;
    top: 340px;
    left: -250px;
    opacity: 0;
    padding: 0;
    margin: 0;
  }
  .text-spiegazione {
      color:white;
      font-family: 'Sen', sans-serif;
      font-size: 1rem;
      line-height: 24px;
      margin-top: 10px;
      padding: 0;
      text-align: justify;
    }
}

</style>

<script>
export default {
  name: 'AboutInfo'
}
</script>
