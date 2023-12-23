<template>
  <section class="sectio about-section">
    <div class="container">
      <div class="row">
        <div class="col-md-5 mt-5">
          <h1 class="section-title mt-5">About Us</h1>

          <p class="font-weight-bold">We’re a team of four passioned people.</p>
          <p>
            We’re ready to take the world by storm and let you find new travel
            opportunities. Our everyday task is to make sure that you satisfied
            with the services and products that we provide.
          </p>
          <p class="font-weight-bold">With 💖 from Amsterdam, Netherlands.</p>

          <button type="button" class="btn btn-primary mt-4 text-uppercase">Read more about us</button>
        </div>

        <div class="col-md-7 p-5">
          <div class=" gallery-container">

          
          <div class="row">
            <div class="col px-0">
              <div class="image-gallery-box">
                <img src="@/assets/images/men.png" class="img-gallery"/>
              </div>
            </div>
            <div class="col px-0">
              <div class="image-gallery-box overlay">
                <img src="@/assets/images/girl1.jpg" class="img-gallery"/>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col px-0">
              <div class="image-gallery-box overlay">
                <img src="@/assets/images/girl23jpg.jpg" class="img-gallery"/>
              </div>
            </div>
            <div class="col px-0">
              <div class="image-gallery-box overlay">
                <img src="@/assets/images/girl2.jpg" class="img-gallery"/>
              </div>
            </div>
            
          </div>
          <div class="gallery-dots">
            <img src="@/assets/images/dots2.svg"/>
            <img src="@/assets/images/dots2.svg"/>
            <img src="@/assets/images/dots2.svg"/>
            <img src="@/assets/images/dots2.svg"/>
          </div>
          
        </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style scoped>

.image-gallery-box{
  width: 100%;
  aspect-ratio : 1 / 1;
  background-size: cover;
  background-position: center;
}

.img-gallery{
  width: 100%;
  aspect-ratio : 1 / 1;
  object-fit: cover;
}

div.overlay{
  position: relative;
}
div.overlay::after{
  content: " ";
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background-color: black;
  opacity: 0.3;
}

.gallery-container{
  position: relative;
}

.gallery-dots{
  position: absolute;
  width: 50px;
  height: auto;
  top: 10%;
  left: calc(100% + 10px);
}
.gallery-dots img{
  margin-bottom: 10px;
}


</style>
