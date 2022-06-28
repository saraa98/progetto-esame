<!-- Please remove this file from your project -->
<template>
  <section class="section section-about">
    <p class="back-home"><NuxtLink to="/"> 
    <svg class="back" width="43" height="32" viewBox="0 0 43 32" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M17.9167 32L20.4429 29.744L6.86208 17.6H43V14.4H6.86208L20.4429 2.256L17.9167 0L0 16L17.9167 32Z" fill="white"/>
    </svg></NuxtLink>Home</p>
    <h1 class="about-intro">About Us</h1>
  </section>
</template>

<style>
  section {
    height: 100vh;
  }

  .section-about {
    background-image: url('../img/bgabout.png');
    background-size: cover;
    background-repeat: no-repeat;
  }
  .back-home {
    position: fixed;
    top: 100px;
    margin-left: 50px;
    color: white !important;
    font-family: 'Fraunces', serif;
    font-style: italic;
    font-weight: lighter;
    font-size: 1.2rem;
    z-index: 999;
  }
  .back {
    width: 28px;
    height: auto;
    margin-right: 10px;
  }

  h1 {
    font-family: 'Fraunces', serif;
    font-size: 4rem;
    font-style: italic;
    font-weight: 700;
    text-align: center;
    color: white;
    position: relative;
    top: 300px;
  }

  .about-intro {
    opacity: 0;
  }
  
</style>

<script>
export default {
  name: 'Aboutintro'
}
</script>
