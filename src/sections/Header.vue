<template>
  <header class="header">
    <div
      class="container d-flex h-100 align-items-center justify-content-center"
    >
      <div class="row w-100">
        <div class="col-md-6 text-center">
          <h1 class="my-0 header-title">Night Trips</h1>
          <h6 class="text-white mx-auto mt-2 mb-5 header-subtitle">
            WE GOT TRIPS FOR THE TRIPPSTER IN YOU
          </h6>
          <p class="text-white">
            Neque, eros commodo, nascetur ullamcorper vitae. Tincidunt ut
            venenatis, volutpat lorem ut faucibus mauris, quisque. Integer
            gravida sed quis congue. Vel risus, arcu a viverra leo id pulvinar
            ultricies. Enim in in in pulvinar nulla sollicitudin. Ullamcorper.
          </p>
        </div>
      </div>
    </div>
    <div class="container d-flex align-items-center justify-content-between mt-5">

      <div class="scroll-btn">
        <div class="d-flex align-items-center">
          SCROLL 
          <div class="line">

          </div></div> 
      </div>
      <div class="">
        <p>
          <a href="" class="mr-4">
            <img src="@/assets/images/instagram.svg" class="social-image"
          /></a>
        </p>
        <p>
          <a href="" class="mr-4">
            <img src="@/assets/images/facebook.svg" class="social-image"
          /></a>
        </p>
        <p>
          <a href="" class="mr-4">
            <img src="@/assets/images/twitter.svg" class="social-image"
          /></a>
        </p>
      </div>
    </div>
  </header>
</template>

<script setup></script>

<style scoped>
.header-subtitle {
  letter-spacing: 2px;
  margin-top: 10px;
}

.line{
  width: 80px;
  height: 2px;
  border-radius: 13px;
  margin-left: 10px;
background: linear-gradient(180deg, #09F4F4 0%, #00C9E0 100%);
}
.scroll-btn{
  transform: rotate(-90deg);
}
</style>
