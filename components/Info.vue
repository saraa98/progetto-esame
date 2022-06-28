<!-- Please remove this file from your project -->
<template>
  <section class="section section-two">
      <div class="items">
          <div class="item1">
              <p class="tag_title"><svg width="80" height="2" style="margin-right: 10px;" viewBox="0 0 80 2" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <line y1="1" x2="106" y2="1" stroke="#BDC4E4" stroke-width="1.5"/>
                </svg>Flowery</p>
              <h2 class="our-services">Our services</h2>
              <p class="text-services">Changing seasons, festivals, holidays, and special celebrations often call for different varieties of flowers. Firmly rooted in the floral field, we can assist with the best selection for you and your peace of mind. Our team of highly qualified and trained experts know exactly how to break down a design to provide you...</p>
              <button class="read-services">READ MORE</button>
          </div>
          <img class="flower_service" src="../img/flower.jpg" />
      </div>
  </section>
</template>

<style>
.section-two {
   height: 67vh;
   background-color: white;
 }

.items {
  display: flex;
  justify-content: space-between;
}

.item1{
  position: relative;
  top: 90px;
  margin-left: 60px;
  margin-right: 60px;
}

h2 {
  font-family: 'Fraunces', serif;
  font-size: 2.5rem;
  font-weight: 600;
  color: #8B9EFF;
  margin-top: 15px;
  margin-bottom: 10px;
}

.our-services {
  opacity: 0;
}

.text-services {
  font-family: 'Sen', sans-serif;
  font-size: 1rem;
  margin-bottom: 25px;
  opacity: 0;
}

.flower_service {
  width: 720px;
  height: auto;
  opacity: 0;
}

.tag_title {
  font-family: 'Fraunces', serif;
  font-size: 1.5rem;
  font-weight: 600;
  font-style: italic;
  color: #BDC4E4;
  margin: 0;
  opacity: 0;
}

.read-services {
  width: 230px;
  height: 48px;
  text-align: center;
  font-family: 'Fraunces', serif;
  background-color: white;
  color:#8B9EFF;
  border: 2px solid #8B9EFF;
  transition: 0.8s;
  opacity: 0;
}

.read-services:hover {
  background-color:#8B9EFF;
  color:white;
}
@media (max-width: 768px){
  
  .section-two {
    height: 100vh;
    background-color: white;
  }

  .items {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  .item1{
  position: relative;
  top: 40px;
  margin-left: 60px;
  margin-right: 60px;
  margin-bottom: 60px;
}
.flower_service {
  width: 520px;
  height: auto;
  opacity: 0;
}
}
</style>


<script>
export default {
  name: 'Info',
}
</script>