<!-- Please remove this file from your project -->
<template>
  <section class="section section-details">
    <p class="back-home"><NuxtLink to="/"> 
    <svg class="back" width="43" height="32" viewBox="0 0 43 32" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M17.9167 32L20.4429 29.744L6.86208 17.6H43V14.4H6.86208L20.4429 2.256L17.9167 0L0 16L17.9167 32Z" fill="white"/>
    </svg></NuxtLink>Home</p>
    <div class="details">
      <img class="img_details" src="../img/rose.jpg" />
      <div class="title_details">
        <p class="tag-img-rose"><svg width="60" height="2" style="margin-right: 10px;" viewBox="0 0 60 2" fill="none" xmlns="http://www.w3.org/2000/svg">
                <line y1="1" x2="106" y2="1" stroke="#BDC4E4" stroke-width="1.5"/> </svg>roses</p>
        <h2 class="title-img-rose">Purple Roses</h2>
        <p class="text-img-rose">The Purple Roses are a dainty, soft and gentle flowers, known to symbolise appreciation, gratitude and traditional values. They make a great addition to weddings and other once-in-a-lifetime events.Pair a Lisianthus with wax flowers or Scabiosa to bring out a fresh, lively look. </p>
        <button class="order">PRE-ORDER</button>
        <div class="elenco-descrizione">
          <ul class="elenco elenco1">
            <li>Color</li>
            <li>Price</li>
            <li>Availability</li>
          </ul>
          <ul class="elenco elenco2">
            <li>Purple</li>
            <li>5€ to 25€</li>
            <li>Spring, Summer</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style>

.section-details {
  height: 100vh;
  background-color:#0E0F12;
  color: white;
}
.details {
  display: flex;
  justify-content: center;
  position: relative;
  top: 175px;
  margin-right: 200px;
  margin-left: 200px;
}

.tag-img-rose {
  color: #BDC4E4;
  font-family: 'Fraunces', serif;
  font-size: 1.1rem;
  margin-bottom: 3px;
  opacity: 0;
}

.title-img-rose {
  font-family: 'Fraunces', serif;
  font-size: 2.5rem;
  font-style: italic;
  font-weight: 600;
  margin-top: 5px;
  margin-bottom: 15px;
  opacity: 0;
}

.text-img-rose {
  font-family: 'Sen', sans-serif;
  font-size: 1rem;
  line-height: 22px;
  opacity: 0;
}

.img_details {
  width: 600px;
  height: auto;
  margin-right: 60px;
  border: 0.5px solid #BDC4E4;
  opacity: 0;
}

.order{
  width: 210px;
  height: 44px;
  text-align: center;
  font-family: 'Fraunces', serif;
  background-color:black;
  color:#8B9EFF;
  border: 2px solid #8B9EFF;
  font-family: 'Fraunces', serif;
  font-size: 1.2rem;
  margin-top: 10px;
  margin-bottom: 10px;
  opacity: 0;
}


.elenco li {
  display: block;
  text-decoration: none;
  font-size: 1rem;
}

.elenco-descrizione {
  display: flex;
  justify-content: space-between;
  opacity: 0;
}

.elenco {
  padding: 0;
  margin-top: 20px;
}

.elenco1 li{
  font-family: 'Fraunces', serif;
  color: #BDC4E4;
  font-style: italic;
  font-weight: 400;
}
.elenco2 li{
  font-family: 'Sen', sans-serif;
  color: white;
  position: relative;
  left: -100px;
  line-height: 23px;
}

@media (max-width: 768px) {
  .section-details {
  height: 140vh;
  background-color:#0E0F12;
  color: white;
}
  .details {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  position: relative;
  top: 175px;
  margin-right: 200px;
  margin-left: 200px;
}
.img_details {
  width: 400px;
  height: auto;
  border: 0.5px solid #BDC4E4;
  opacity: 0;
  margin-top: 26px;
  margin-left: 50px;
  margin-bottom: 20px;
}
.tag-img-rose {
  color: #BDC4E4;
  font-family: 'Fraunces', serif;
  font-size: 1.1rem;
  margin-bottom: 3px;
  opacity: 0;
}
.title-img-rose {
  font-family: 'Fraunces', serif;
  font-size: 2rem;
  font-style: italic;
  font-weight: 600;
  margin-top: 5px;
  margin-bottom: 15px;
  opacity: 0;
}
.text-img-rose {
  font-family: 'Sen', sans-serif;
  font-size: 0.9rem;
  line-height: 26px;
  text-align: justify;
  opacity: 0;
}
.elenco li {
  display: block;
  text-decoration: none;
  font-size: 0.8rem;
}
.elenco2 li{
  font-family: 'Sen', sans-serif;
  color: white;
  position: relative;
  left: 10px;
  line-height: 23px;
}

}
 
</style>

<script>
export default {
  name: 'InfoDettaglio'
}
</script>
