<template>
  <div class="swiper swiper-overflow py-5">
    <div class="container">
      <div id="slider-gallery-16" class="swiper-container row">
        <div class="swiper-wrapper">
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
          <div class="swiper-slide col-11 col-md-3">
            <img class="w-100" src="@/assets/pictures/image-540x540.png">
          </div>
        </div>
      </div><a id="slider-gallery-16-prev" class="carousel-control-prev carousel-control-outside" href="">
        <div class="carousel-control-prev-icon" />
      </a><a id="slider-gallery-16-next" class="carousel-control-next carousel-control-outside" href="">
        <div class="carousel-control-next-icon" />
      </a>
    </div>
  </div>
</template>

<script>
/*
  var mySwiper16 = new Swiper('#slider-gallery-16', {
    speed: 400,
    navigation: {
      nextEl: '#slider-gallery-16-next',
      prevEl: '#slider-gallery-16-prev',
    },
    pagination: {
      el: '#slider-gallery-16-pagination',
      clickable: true
    },
    slidesPerView: 'auto',
    slideToClickedSlide: true
  });

  $(mySwiper16.slides).each(function() {
    $(this).on('click', function() {
      if (mySwiper16.activeIndex >= $(this).index()) {
        mySwiper16.slidePrev();
      } else {
        mySwiper16.slideNext();
      }
    });
  });
*/
export default {
  name: 'Gallery16'
}
</script>
