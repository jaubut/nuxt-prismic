<template>
  <div class="container">
    <div class="navbar navbar-expand-lg justify-content-between">
      <div class="d-lg-none">
        <img class="navbar-toggler mr-1" src="@/assets/glyphs/burger.svg" @click="MenuShow=!MenuShow">
      </div>
      <div>
        <img src="@/assets/logos/cr-logo-type-white.svg" width="32" alt="">
      </div>
      <div class="collapse navbar-collapse flex-grow-0 weight-500">
        <div class="navbar-nav">
          <div class="nav-item">
            <a class="nav-link text-white pl-0" href="#apropos">À propos</a>
          </div>
          <div class="nav-item">
            <a class="nav-link text-white" href="#ressource">Services</a>
          </div>
          <!--
          <div class="nav-item"><a class="nav-link text-dark" href="">Third</a></div>
          <div class="nav-item"><a class="nav-link text-dark" href="">Fourth</a></div>
          <div class="nav-item"><a class="nav-link text-dark" href="">Fifth</a></div>
          <div class="nav-item"><a class="nav-link text-dark" href="">Sixth</a></div>
          <div class="nav-item d-none d-lg-block"><a class="nav-link text-dark pr-0" href=""><img src="@/assets/glyphs/search.svg" /></a></div>
          -->
        </div>
      </div>
      <div class="d-lg-none ml-auto">
        <!--
        <div class="nav-item"><a class="nav-link text-dark pr-0" href=""><img src="@/assets/glyphs/search.svg" /></a></div>-->
      </div>
    </div>
    <transition name="slide-fade">
      <div v-if="MenuShow" id="menu-4-sidebar" class="navbar-side show" @click="MenuShow=!MenuShow">
        <div class="navbar-side-content d-flex flex-column justify-content-between">
          <div class="weight-700">
            <img style="cursor: pointer;" class="navbar-side-close mb-4" src="@/assets/glyphs/close.svg" width="32">
            <div class="navbar-nav">
              <div class="nav-item">
                <a class="nav-link pl-0" href="#apropos">À propos</a>
              </div>
              <div class="nav-item">
                <a class="nav-link" href="#ressource">Services</a>
              </div>
              <!--
              <div class="nav-item d-none d-lg-block"><a class="nav-link text-dark pr-0" href=""><img src="@/assets/glyphs/search.svg" /></a></div>-->
            </div>
          </div>
          <div>
            <p class="mb-3">
              <a class="transparent-invert-link ml-2" target="_blank" href="https://www.facebook.com/cultureduroyaume"><i class="fab fa-facebook-square" /></a>
            </p>
            <p class="small mb-0">
              <span class="d-block d-xl-inline text-muted mb-1 mb-xl-0 mr-2">&copy; 2020 Culture du Royaume. Tout droit réservé.</span>
            </p>
          </div>
        </div>
        <div class="navbar-side-content weight-700">
          <a class="navbar-side-close mb-4" href=""><img src="@/assets/glyphs/close.svg" width="32"></a>
        </div>
      </div>
    </transition>
  </div>
</template>

<script>
/*
  $(function() {
    $('[data-id=menu-4-sidebar-toggle]').click(function(e) {
      eDefault();
      $('#menu-4-sidebar').toggleClass('show');
    });

    $('[data-id=menu-4-sidebar-close]').click(function(e) {
      eDefault();
      $('#menu-4-sidebar').removeClass('show');
    });
  });
*/
export default {
  name: 'Menu4',
  data () {
    return {
      MenuShow: false
    }
  }
}
</script>

<style scoped>
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .2s ease;
}
.slide-fade-enter {
  transform: translateX(-50px);
  opacity: 0;
}
.slide-fade-leave-to {
 transform: translateX(-50px);
  opacity: 0;
}
</style>
