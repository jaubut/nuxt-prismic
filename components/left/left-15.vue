<template>
  <div class="container">
    <div class="row justify-content-between align-items-center py-5">
      <div class="col-12 col-md-5 order-2 order-md-1">
        <h3>Medium length headline</h3>
        <p class="mb-4">
          Change the color to match your brand or vision, add your logo, choose the perfect thumbnail, remove the playbar, add speed controls, and more. Increase engagement with CTAs and custom end screens, or keep your video private and password-protected.
        </p>
        <div class="row">
          <div class="col-6">
            <div class="price-large mb-1">
              32<span class="price-unit ml-1">GB</span>
            </div>
            <div class="small">
              Gorgeous, high-quality video sharing on desktop, mobile, tablet
            </div>
          </div>
          <div class="col-6">
            <div class="price-large mb-1">
              2.6<span class="price-unit ml-1">Million</span>
            </div>
            <div class="small">
              Gorgeous, high-quality video sharing on desktop, mobile, tablet
            </div>
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 order-1 order-md-2 pl-md-0 mb-4 mb-md-0">
        <div class="swiper has-outside-pagination">
          <div id="slider-left-15" class="swiper-container">
            <div class="swiper-wrapper">
              <div class="swiper-slide">
                <img class="w-100" src="@/assets/pictures/image-555x380.png">
              </div>
              <div class="swiper-slide">
                <img class="w-100" src="@/assets/pictures/image-555x380.png">
              </div>
              <div class="swiper-slide">
                <img class="w-100" src="@/assets/pictures/image-555x380.png">
              </div>
            </div>
          </div>
          <div id="slider-left-15-pagination" class="swiper-pagination swiper-pagination-outside" /><a id="slider-left-15-prev" class="carousel-control-prev" href="">
            <div class="carousel-control-prev-icon" />
          </a><a id="slider-left-15-next" class="carousel-control-next" href="">
            <div class="carousel-control-next-icon" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/*
  var mySwiper = new Swiper('#slider-left-15', {
    speed: 400,
    navigation: {
      nextEl: '#slider-left-15-next',
      prevEl: '#slider-left-15-prev',
    },
    pagination: {
      el: '#slider-left-15-pagination',
      clickable: true
    }
  });
*/
export default {
  name: 'Left15'
}
</script>
