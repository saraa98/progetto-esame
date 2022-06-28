<!-- Please remove this file from your project -->
<template>
  <section class="section section-about-awards">
    <hr class="hr" color="#BDC4E4" width="80%">
    <div class="row-awards">
      <div class="awards award-one">
        <img class="medaglia" src="../img/medaglia.svg" />
        <h2 class="title-trofeo">Best Flowers</h2>
        <h5 class="subtitle">Since 1998</h5>
      </div>
      <div class="awards award-two">
        <img class="medaglia" src="../img/verificato.svg" />
        <h2 class="title-trofeo">1° in the World</h2>
        <h5 class="subtitle">June 1987</h5>
      </div>
      <div class="awards award-three">
        <img class="medaglia" src="../img/trofeo.svg" />
        <h2 class="title-trofeo">FC Champions</h2>
        <h5 class="subtitle">May 2008</h5>
      </div>
    </div>
   <hr class="hr" color="#BDC4E4" width="80%">
  </section>
</template>

<style>

  .section-about-awards {
    background-color: #0E0F12;
    height: 50vh;
  }

   hr {
    margin: 0 auto;
    border: 0.8px solid;
  } 

  .hr {
    opacity: 0;
  }

  .row-awards {
    display: flex;
    justify-content: space-evenly;
    margin-top: 40px;
    margin-bottom: 40px;
    opacity: 0;
  }

  .awards {
    text-align: center;
  }

  .medaglia {
    height: 122px;
    width: auto;
  }

  .title-trofeo {
    font-family: 'Fraunces', serif;
    font-size: 2rem;
    font-weight: 500;
    font-style: italic;
    color: #8B9EFF;
    margin-top: 30px;
  }

  .subtitle {
    font-family:'Sen', sans-serif;
    font-size: 1rem;
    color: white;
    font-style: normal;
  }

  @media (max-width: 768px){
    .medaglia {
    height: 70px;
    width: auto;
  }
  .title-trofeo {
    font-family: 'Fraunces', serif;
    font-size: 1.2rem;
    font-weight: 500;
    font-style: italic;
    color: #8B9EFF;
    margin-top: 30px;
  }

  .subtitle {
    font-family:'Sen', sans-serif;
    font-size: 0.8rem;
    color: white;
    font-style: normal;
    margin-top: 40px;
    margin-bottom: 0px;
  }

  }

</style>

<script>
export default {
  name: 'Awards'
}
</script>
