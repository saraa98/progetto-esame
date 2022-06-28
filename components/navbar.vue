<!-- Please remove this file from your project -->
<template>
  <nav id="nav">
    <img class="logo" src="../img/logo1.png" />
    <ul class="voci_menu">
      <li><NuxtLink to="/about">ABOUT</NuxtLink></li>
      <li>SERVICES</li>
      <li>CONTACTS</li>
    </ul>
  </nav>
</template>

<style>
  #nav {
    padding-top: 10px;
    padding-left: 25px;
    padding-right: 25px;
    position: fixed;
    width: 100%;
    z-index: 999;
    background-color: transparent;
    display: flex;
    justify-content: space-between;
    align-items: baseline;
  }

.logo {
    width: 135px;
    height: auto;
  }

  li {
    display: inline;
    text-decoration: none;
    margin-right: 20px;
    color: #BDC4E4;
    font-family: 'Sen', sans-serif;
    font-size: 1.25rem;
  }

  @media (max-width: 768px) {
    #nav {
    padding-top: 10px;
    padding-left: 25px;
    padding-right: 25px;
    position: fixed;
    width: 100%;
    z-index: 999;
    background-color: transparent;
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    }

    li {
    display: inline;
    text-decoration: none;
    margin-right: 10px;
    color: #BDC4E4;
    font-family: 'Sen', sans-serif;
    font-size: 1rem;
    }
  }

</style>




<script>
export default {
  name: 'navbar'
}
</script>
