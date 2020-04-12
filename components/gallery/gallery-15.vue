<template>
  <div class="swiper swiper-overflow py-5">
    <div class="container">
      <div id="slider-gallery-15" class="swiper-container row">
        <div class="swiper-wrapper">
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-4">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
        </div>
      </div><a id="slider-gallery-15-prev" class="carousel-control-prev carousel-control-outside" href="">
        <div class="carousel-control-prev-icon" />
      </a><a id="slider-gallery-15-next" class="carousel-control-next carousel-control-outside" href="">
        <div class="carousel-control-next-icon" />
      </a>
    </div>
  </div>
</template>

<script>
/*
var mySwiper15 = new Swiper('#slider-gallery-15', {
    speed: 400,
    navigation: {
      nextEl: '#slider-gallery-15-next',
      prevEl: '#slider-gallery-15-prev',
    },
    pagination: {
      el: '#slider-gallery-15-pagination',
      clickable: true
    },
    slidesPerView: 'auto'
  });

  $(mySwiper15.slides).each(function() {
    $(this).on('click', function() {
      if (mySwiper15.activeIndex >= $(this).index()) {
        mySwiper15.slidePrev();
      } else {
        mySwiper15.slideNext();
      }
    });
  });
*/
export default {
  name: 'Gallery15'
}
</script>
