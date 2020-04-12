<template>
  <div class="container">
    <div class="row justify-content-center py-5">
      <div class="col-12 col-md-8 col-lg-6">
        <div class="swiper has-outside-pagination">
          <div id="slider-gallery-13" class="swiper-container">
            <div class="swiper-wrapper">
              <div class="swiper-slide">
                <div class="images-ratio ratio-4-3" style="background-image: url(@/assets/pictures/image-555x380.png)" />
              </div>
              <div class="swiper-slide">
                <div class="images-ratio ratio-4-3" style="background-image: url(@/assets/pictures/image-555x380.png)" />
              </div>
              <div class="swiper-slide">
                <div class="images-ratio ratio-4-3" style="background-image: url(@/assets/pictures/image-555x380.png)" />
              </div>
            </div>
          </div>
          <div id="slider-gallery-13-pagination" class="swiper-pagination swiper-pagination-outside" /><a id="slider-gallery-13-prev" class="carousel-control-prev carousel-control-outside" href="">
            <div class="carousel-control-prev-icon" />
          </a><a id="slider-gallery-13-next" class="carousel-control-next carousel-control-outside" href="">
            <div class="carousel-control-next-icon" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/*
var mySwiper13 = new Swiper('#slider-gallery-13', {
    speed: 400,
    navigation: {
      nextEl: '#slider-gallery-13-next',
      prevEl: '#slider-gallery-13-prev',
    },
    pagination: {
      el: '#slider-gallery-13-pagination',
      clickable: true
    },
    slidesPerView: 'auto'
  });
*/
export default {
  name: 'Gallery13'
}
</script>
