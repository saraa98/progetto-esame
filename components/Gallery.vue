<!-- Please remove this file from your project -->
<template>
  <section class="section section-three">
    <div class="general_title">
      <p class="tag_title2"><svg width="80" height="2" style="margin-right: 10px;" viewBox="0 0 80 2" fill="none" xmlns="http://www.w3.org/2000/svg">
                <line y1="1" x2="106" y2="1" stroke="#BDC4E4" stroke-width="1.5"/>
          </svg>Flowery</p>
      <h2 class="new-entry">New Entry</h2>
    </div>
        <div class="section-carousel">
          <div class="section-preview">
           <img src="../img/violet.jpg" />
            <span><p><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
          <line y1="1" x2="106" y2="1" stroke="white" stroke-width="1.5"/> </svg>Discover <br> more</p></span>
          </div>
          <div class="section-preview">
             <NuxtLink to="/details"><img src="../img/rose.jpg" />
            <span><p><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
          <line y1="1" x2="106" y2="1" stroke="white" stroke-width="1.5"/> </svg>Discover <br> more</p></span></NuxtLink>
          </div>
          <div class="section-preview"> 
            <img src="../img/prime.jpg" />
            <span><p><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
          <line y1="1" x2="106" y2="1" stroke="white" stroke-width="1.5"/> </svg>Discover <br> more</p></span>
          </div>
        </div>
  </section>
</template>

<style>
  .section-three {
    height: 80vh;
    background-color: #F9F6FF;
  }
  .general_title {
    position: relative;
    top: 70px;
    margin-left: 50px;
  }

  .tag_title2 {
  font-family: 'Fraunces', serif;
  font-size: 1.5rem;
  font-weight: 600;
  font-style: italic;
  color: #BDC4E4;
  margin: 0;
  opacity: 0;
}

.new-entry {
  opacity: 0;
}

  .section-carousel{
    display: flex;
    justify-content: center;
    position: relative;
    top: 100px;
    opacity: 0;
  }
  .section-preview{
    margin: 20px;
    z-index: 0;
  }

  .section-carousel img {
    width: 400px;
    height: 250px;
    transition: 0.6s;
  }

  .section-preview span p {
    opacity: 0;
    text-align: center;
    color: white;
    width: 100%;
    font-family: 'Fraunces', serif;
    font-size: 2rem;
    line-height: 24px;
    text-shadow: 2px 2px black;
    position: relative;
    top: -145px;
    z-index: 998;
    transition: 0.6s;
  }
  .section-preview:hover span p{
    opacity: 1;
  } 

  .section-preview:hover img {
    filter: blur(1px);
    border-radius: 32px;
  }

 @media (max-width: 768px) {
  .section-three {
    height: 150vh;
    background-color: #F9F6FF;
  }
  
  .section-carousel{
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    position: relative;
    top: 100px;
    opacity: 0;
   }
  .section-preview{
    margin: 5px;
    z-index: 0;
  }

  .section-carousel img {
    width: 350px;
    height: 218.75px;
    transition: 0.6s;
  }
  .section-preview span p {
    opacity: 0;
    text-align: center;
    color: white;
    width: 100%;
    font-family: 'Fraunces', serif;
    font-size: 2rem;
    line-height: 24px;
    text-shadow: 2px 2px black;
    position: relative;
    top: -125px;
    z-index: 998;
    transition: 0.6s;
  }
  .section-preview:hover span p{
    opacity: 1;
  } 
 } 

</style>

<script>
export default {
  name: 'Gallery'
}
</script>
