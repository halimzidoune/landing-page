<template>
  <nav class="navbar navbar-expand-lg navbar-light fixed-top" id="mainNav">
    <div class="container px-4 px-lg-5 d-flex align-items-center">
      <a class="navbar-brand header-logo mt-2" href="#page-top">NT.</a>
      <button
        class="navbar-toggler navbar-toggler-right"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarResponsive"
        aria-controls="navbarResponsive"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        Menu
        <svg
          class="svg-inline--fa fa-bars"
          aria-hidden="true"
          focusable="false"
          data-prefix="fas"
          data-icon="bars"
          role="img"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 448 512"
          data-fa-i2svg=""
        >
          <path
            fill="currentColor"
            d="M0 96C0 78.3 14.3 64 32 64H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32C14.3 128 0 113.7 0 96zM0 256c0-17.7 14.3-32 32-32H416c17.7 0 32 14.3 32 32s-14.3 32-32 32H32c-17.7 0-32-14.3-32-32zM448 416c0 17.7-14.3 32-32 32H32c-17.7 0-32-14.3-32-32s14.3-32 32-32H416c17.7 0 32 14.3 32 32z"
          ></path></svg
        ><!-- <i class="fas fa-bars"></i> Font Awesome fontawesome.com -->
      </button>

      <div class="collapse navbar-collapse" id="navbarResponsive">
        <ul class="navbar-nav ms-auto d-flex align-items-center">
          <li class="nav-item mr-4">
            <img src="@/assets/images/search 1.svg" width="40" class="search"/>
          </li>
          <li class="nav-item">
            <button type="button" class="btn btn-primary mt-4 ml-5 text-uppercase">MENU</button>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style soped>
  .search{
    margin-right: 20px;
    margin-top: 25px;
  }
</style>
