<script setup>
import { onMounted, ref, onUpdated } from 'vue'

const academic = ref([
  {
    icon: 'fa fa-graduation-cap',
    title: 'Formación Académica',
    content: 'Universidad Centroccidental Lisandro Alvarado (UCLA) — Ingeniería Informática (en curso)'
  },
  {
    icon: 'fa fa-cogs',
    title: 'Tecnologías',
    content: 'HTML, CSS, JavaScript, C#, .NET, Entity Framework, Angular, Vue.js'
  },
  {
    icon: 'fa fa-briefcase',
    title: 'Experiencia Profesional',
    content: 'Mpsoft (Desarrollador Junior), Tester independiente, Ayudante de albañilería, Atención al cliente'
  },
  {
    icon: 'fa fa-book',
    title: 'Educación Complementaria',
    content: 'Platzi: Fundamentos de .NET, Vue.js, Testing, Git y GitHub, HTML/CSS/JS Práctico'
  }
])

const carouselItems = ref([
  {
    icon: 'fa fa-code',
    title: 'Frontend Developer',
    content: 'Diseño y construcción de interfaces modernas usando Vue.js, HTML, CSS y JavaScript.'
  },
  {
    icon: 'fa fa-database',
    title: 'Backend Developer',
    content: 'Desarrollo de lógica de negocio con C#, .NET y acceso a datos usando Entity Framework.'
  },
  {
    icon: 'fa fa-users',
    title: 'Trabajo en Equipo',
    content: 'Experiencia en entornos colaborativos y metodologías ágiles.'
  },
  {
    icon: 'fa fa-wrench',
    title: 'Testing & QA',
    content: 'Pruebas funcionales y control de calidad para garantizar la estabilidad del software.'
  },
  {
    icon: 'fa fa-lightbulb-o',
    title: 'Solución de Problemas',
    content: 'Habilidad para enfrentar retos técnicos con creatividad y pensamiento lógico.'
  }
])

onMounted(() => {
  $(".curriculum-slider").owlCarousel({
    loop: true,
    items: 3,
    dots: true,
    nav: false,
    smartSpeed: 1000,
    autoHeight: false,
    touchDrag: true,
    mouseDrag: true,
    margin: 30,
    autoplay: true,
    slideSpeed: 600,
    responsive: {
      0: { items: 1, nav: false, dots: false },
      600: { items: 2, nav: false, dots: false },
      768: { items: 2, nav: false, dots: false },
      1100: { items: 3, nav: false, dots: true }
    }
  })
})
</script>

<template>
  <div id="curriculum" class="services-area gray-bg section-padding pad-bot-90">
    <div class="container">
      <div class="row">
        <div class="offset-lg-2 col-lg-8 text-center">
          <div class="section-title">
            <h6><i class="fa fa-briefcase"></i> Currículum</h6>
           <h2>Mi Experiencia en Desarrollo y <b>Habilidades Full-Stack</b></h2>
          </div>
        </div>
      </div>

      <!-- Carrusel profesional -->
      <div class="row mt-30">
        <div class="col-lg-12">
          <div class="curriculum-slider owl-carousel">
            <div class="single-service-area" v-for="(item, index) in carouselItems" :key="index">
              <div class="service-icon">
                <i :class="item.icon"></i>
              </div>
              <h5>{{ item.title }}</h5>
              <p>{{ item.content }}</p>
            </div>
          </div>
        </div>
      </div>

      <!-- Información detallada -->
      <div class="row mt-5">
        <div class="col-md-6 mb-4" v-for="(item, index) in academic" :key="index">
          <div class="single-service-area">
            <div class="service-icon">
              <i :class="item.icon"></i>
            </div>
            <h5>{{ item.title }}</h5>
            <p>{{ item.content }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.section-title h6 i {
  margin-right: 8px;
}
.single-service-area {
  background: #fff;
  border-radius: 10px;
  padding: 20px;
  box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}
.single-service-area:hover {
  transform: translateY(-5px);
}
.service-icon {
  font-size: 24px;
  color: #0056b3;
  margin-bottom: 10px;
  display: block;
  text-align: center;
}
</style>
