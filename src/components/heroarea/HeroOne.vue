<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  $('.homepage-slides').owlCarousel({
    items: 1,
    dots: false,
    nav: true,
    loop: true,
    autoplay: true,
    autoplayTimeout: 5000,
    smartSpeed: 2000,
    slideSpeed: 600,
    animateOut: 'fadeOut',
    navText: [
      "<i class='la la-angle-left'></i>",
      "<i class='la la-angle-right'></i>"
    ],
    responsive: {
      0: { items: 1, nav: false, dots: false },
      600: { items: 1, nav: false, dots: false },
      768: { items: 1, nav: false, dots: false },
      1100: { items: 1, nav: true, dots: false }
    }
  });

  $(".homepage-slides").on("translate.owl.carousel", function () {
    $(".single-slide-item h1").removeClass("animated fadeInUp").css("opacity", "1");
    $(".single-slide-item h6").removeClass("animated fadeInDown").css("opacity", "1");
    $(".single-slide-item p").removeClass("animated fadeInDown").css("opacity", "1");
    $(".single-slide-item a.main-btn").removeClass("animated fadeInDown").css("opacity", "1");
  });

  $(".homepage-slides").on("translated.owl.carousel", function () {
    $(".single-slide-item h1").addClass("animated fadeInUp").css("opacity", "1");
    $(".single-slide-item h6").addClass("animated fadeInDown").css("opacity", "1");
    $(".single-slide-item p").addClass("animated fadeInDown").css("opacity", "1");
    $(".single-slide-item a.main-btn").addClass("animated fadeInDown").css("opacity", "1");
  });
});
</script>

<template>
  <!-- CAMBIO AQUÍ: id="sobre-mi" -->
  <div id="home" class="homepage-slides owl-carousel">
    <!-- Slide principal -->
    <div class="single-slide-item">
      <div class="overlay"></div>
      <div class="hero-area-content">
        <div class="container">
          <div class="row justify-content-center">
            <div class="col-lg-12 wow fadeInUp animated" data-wow-delay=".2s">
              <div class="section-title text-center">
                <h6 class="text-white">Jefferson Martinez Castillo</h6>
                <h1>Full-Stack Developer • Baterista • Cristiano</h1>
                <p>
                  Construyo soluciones digitales con pasión, marco el ritmo con mi batería<br />
                  y vivo cada línea de código como una expresión de mi fe en Cristo.
                </p>
              </div>
              <button class="main-btn">Conóceme</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Slide adicional -->
    <div class="single-slide-item hero-area-bg-2">
      <div class="overlay"></div>
      <div class="hero-area-content">
        <div class="container">
          <div class="row justify-content-center">
            <div class="col-lg-12 wow fadeInUp animated" data-wow-delay=".2s">
              <div class="section-title text-center">
                <h6 class="text-white">Trabajo con propósito</h6>
                <h1>Desarrollo software<br />con pasión, precisión y propósito</h1>
                <p>
                  Creo sistemas funcionales, limpios y humanos.<br />
                  No solo escribo código, construyo experiencias que impactan vidas.
                </p>
              </div>
              <button class="main-btn">Learn More</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
