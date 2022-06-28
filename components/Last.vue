<!-- Please remove this file from your project -->
<template>
  <footer>
    <div class="last-section">
      <img class="element footer-logo" src="../img/logo1.png" />
      <div class="element contatti"> 
        <h5>Contacts</h5>
          <ul class="info-contatti">
            <li>Via Verdi 63, VR</li>
            <li>+39 4562981327</li>
            <li>info@flowers.it</li>
          </ul>
          <br>
          <ul class="social_icon">
            <li><img src="../img/Instagram.svg" /></li>
            <li><img src="../img/Facebook.svg" /></li>
            <li><img src="../img/Twitter.svg" /></li>
          </ul>
      </div>
      <div class="element newsletter">
        <h5 class="title-newsletter">Our Newsletter</h5>
        <p class="info-newsletter">Write your e-mail to receive all the news</p>
        <form action="input_iscrizione" class="form1">
          <input type="text" id="mail" placeholder="mario@gmail.com"><NuxtLink to="/"><button v-on:click="onClickButton" class="button_iscrizione">Subscribe</button></NuxtLink>
        </form>
      </div>
    </div>
  </footer>
</template>

<style>
  footer{
    height: 50vh;
    background-color: black;
  }

  .last-section {
    display: flex;
    justify-content: space-evenly;
    padding-top: 30px;
  }

  .last-section .element {
    margin: 60px;
    margin-bottom: 0;
  }

  h5 {
    color: #8B9EFF;
    font-family: 'Fraunces', serif;
    font-size: 2rem;
    font-style: italic;
    font-weight: 600;
  }

  .footer-logo {
    width: auto;
    height: 80px;
    margin-top: 100px !important;
  }

  .info-contatti {
    padding: 0;
    margin-top: 15px;
  }

  .social_icon {
    padding: 0;
  }

  .info-contatti li{
    text-decoration: none;
    display: block;
    color: white;
    font-family: 'Sen', sans-serif;
    font-size: 1rem;
    margin-bottom: 6px;
  }

  .info-newsletter{
    margin-top: 15px;
    margin-bottom: 0;
    color: white;
    font-family: 'Sen', sans-serif;
    font-size: 1rem;
  }

  .form1 {
    margin-top: 5px; 
    padding-right: 15px;
  }
  ::placeholder {
    color:grey;
    font-family: 'Sen', sans-serif;
    font-size: 1rem;
    padding-left: 5px;
  }
  .button_iscrizione {
    width: 100px;
    margin-left: 12px;
    text-align: center;
    font-family: 'Fraunces', serif;
    background-color: #8B9EFF;
    border: 2px solid #8B9EFF;
    color: white;
  }

  @media (max-width: 768px) {
    .last-section {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    padding-top: 0px;
  }
  .footer-logo {
    width: auto;
    height: 40px;
    margin-top: 30px !important;
  }

  .contatti {
    position: relative;
    top: 150px;
  }

  h5 {
    color: #BDC4E4;
    font-family: 'Fraunces', serif;
    font-size: 1rem;
    font-style: italic;
    font-weight: 600;
    position: relative;
    top: -35px;
    text-align: center;
  }
  .info-contatti li{
    text-decoration: none;
    display: inline;
    color: white;
    font-family: 'Sen', sans-serif;
    font-size: 0.8rem;
    position: relative;
    top: -40px;
    margin-bottom: 6px;
    z-index: 998;
  }
   .social_icon {
    position: relative;
    top: -65px;
    left: 110px;
    padding: 0;
  }

  .newsletter {
    position: relative;
    top: -220px;
  }
  .info-newsletter{
    margin-top: 0px;
    margin-bottom: 0;
    color: white;
    font-family: 'Sen', sans-serif;
    font-size: 0.8rem;
  }
  .title-newsletter {
    position: relative;
    top: -5px;
  }
   ::placeholder {
    color:grey;
    font-family: 'Sen', sans-serif;
    font-size: 0.8rem;
    padding-left: 5px;
  }
}
</style>

<script>
export default {
  name: 'Last',
  methods: {
    onClickButton: function() {
      alert('Subscription completed successfully. Welcome to Flowery Family')
    }
  }
}
</script>
