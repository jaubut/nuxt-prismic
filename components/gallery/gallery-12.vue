<template>
  <div class="swiper swiper-overflow py-5">
    <div class="container position-relative">
      <div id="slider-gallery-12" class="swiper-container row">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <div class="col-12">
              <div class="images-ratio ratio-2-1" style="background-image: url(@/assets/pictures/image-1110x540.png)" />
            </div>
          </div>
          <div class="swiper-slide">
            <div class="col-12">
              <div class="images-ratio ratio-2-1" style="background-image: url(@/assets/pictures/image-1110x540.png)" />
            </div>
          </div>
          <div class="swiper-slide">
            <div class="col-12">
              <div class="images-ratio ratio-2-1" style="background-image: url(@/assets/pictures/image-1110x540.png)" />
            </div>
          </div>
        </div>
      </div><a id="slider-gallery-12-prev" class="carousel-control-prev carousel-control-outside" href="">
        <div class="carousel-control-prev-icon" />
      </a><a id="slider-gallery-12-next" class="carousel-control-next carousel-control-outside" href="">
        <div class="carousel-control-next-icon" />
      </a>
    </div>
  </div>
</template>

<script>
/*
  var mySwiper12 = new Swiper('#slider-gallery-12', {
    speed: 400,
    navigation: {
      nextEl: '#slider-gallery-12-next',
      prevEl: '#slider-gallery-12-prev',
    },
    pagination: {
      el: '#slider-gallery-12-pagination',
      clickable: true
    },
    slidesPerView: 'auto'
  });
*/
export default {
  name: 'Gallery12'
}
</script>
