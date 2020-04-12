<template>
  <div class="container">
    <div class="swiper">
      <div id="slider-gallery-11" class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <div class="images-ratio ratio-16-9" style="background-image: url(@/assets/pictures/image-1440x600.png)" />
          </div>
          <div class="swiper-slide">
            <div class="images-ratio ratio-16-9" style="background-image: url(@/assets/pictures/image-1440x600.png)" />
          </div>
          <div class="swiper-slide">
            <div class="images-ratio ratio-16-9" style="background-image: url(@/assets/pictures/image-1440x600.png)" />
          </div>
        </div>
      </div>
      <div id="slider-gallery-11-pagination" class="swiper-pagination" /><a id="slider-gallery-11-prev" class="carousel-control-prev" href="">
        <div class="carousel-control-prev-icon" />
      </a><a id="slider-gallery-11-next" class="carousel-control-next" href="">
        <div class="carousel-control-next-icon" />
      </a>
    </div>
  </div>
</template>

<script>
/*
var mySwiper11 = new Swiper('#slider-gallery-11', {
    speed: 400,
    navigation: {
      nextEl: '#slider-gallery-11-next',
      prevEl: '#slider-gallery-11-prev',
    },
    pagination: {
      el: '#slider-gallery-11-pagination',
      clickable: true
    },
    slidesPerView: 'auto'
  });
 */
export default {
  name: 'Gallery11'
}
</script>
