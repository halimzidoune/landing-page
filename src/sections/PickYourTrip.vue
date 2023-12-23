<template>
  <section class="section">
    <BlurPoint width="500" top="450" left="70" background_color="#41EAD4"/>
    <BlurPoint width="500" top="450" left="70" background_color="#BE41EA"/>
    <BlurPoint width="200" top="450" left="70" background_color="#7741EA"/>

    <BlurPoint width="500" top="450" right="70" background_color="#41EAD4"/>
    <BlurPoint width="500" top="450" right="70" background_color="#BE41EA"/>
    <BlurPoint width="200" top="450" right="70" background_color="#7741EA"/>

    <div class="container">
      <!-- Title section -->
      <div class="row d-flex align-items-center">
        <div class="col-md-5">
          <h1 class="section-title">Pick your trip</h1>
        </div>

        <div class="col-md-7">
          <p>
            Our team put together some trips to you to discover, <br />
            feel free to discover them
          </p>
        </div>
      </div>
      <!-- End Title section -->

      <!-- Tabs -->
      <ul class="nav nav-pills nav-fill mt-100">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Active</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Much longer nav link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" tabindex="-1" aria-disabled="true"
            >Disabled</a
          >
        </li>
      </ul>
      <!-- End Tabs -->
      <div class="mt-100">
        <div class="row">
          <div class="col-md-6">
            <div class="p-4 relative image-container">
              <img src="@/assets/images/dots.svg" class="dots"/>
              <div class="image-box" style=";">

              </div>
              
            </div>
          </div>

          <div class="col-md-6">
            <h1 class="section-title mb-4 mt-5">Chill Adventure</h1>
            <p>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              Accusantium molestiae accusamus ex nulla reiciendis
            </p>

            <p>
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Labore
              odit a velit nobis, odio nostrum aliquam possimus delectus,
              cupiditate ea dolores inventore rerum, excepturi esse voluptas
              laboriosam tempora Lorem, ipsum dolor sit amet consectetur adipisicing elit. Labore
              odit a velit nobis, odio nostrum aliquam possimus delectus,
              cupiditate ea dolores inventore rerum, excepturi esse voluptas
              laboriosam tempor.
            </p>

            <button type="button" class="btn btn-primary mt-4 text-uppercase">See our latest offer</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import BlurPoint from "@/components/BlurPoint.vue";
</script>

<style scoped>
.nav .nav-item a {
  color: rgba(255, 255, 255, 0.5);
  font-weight: bold;
}
.nav-pills .nav-link {
  border-bottom: 2px solid rgba(255, 255, 255, 0.5);
  border-radius: 0;
  padding-top: 12px;
  padding-bottom: 15px;
}
.nav-pills .nav-link.active {
  background: transparent;
  color: #41ead4;
  font-weight: bold;
  border-bottom: 2px solid #41ead4;
}



.image-1{
  width: 80px;
  object-position: center;
}

.image-box{
  width: 400px;
  background-image: url('@/assets/images/image1.jpg');
  background-size: cover;
  background-position: center;
  margin: auto;
  height: 500px;
}

.image-container{
  position: relative;
}

.dots{
  position: absolute;
  width: 100px;
  bottom: 0px;
  left: 80px;
  z-index: -2;
}
</style>
