<script setup>
import { ref } from 'vue'

const features = ref([
  {
    id: 1,
    icon: 'fas fa-cogs',
    title: 'Gestión de Proyectos Industriales',
    content: 'Planificación y control eficiente de proyectos industriales para maximizar la productividad y minimizar riesgos.'
  },
  {
    id: 2,
    icon: 'fas fa-industry',
    title: 'Automatización Industrial',
    content: 'Implementación de sistemas automatizados para optimizar procesos y asegurar calidad en la producción.'
  },
  {
    id: 3,
    icon: 'fas fa-shield-alt',
    title: 'Normas de Seguridad y Calidad',
    content: 'Cumplimiento riguroso de estándares internacionales para garantizar seguridad en el entorno industrial.'
  }
])

const courses = ref([
  {
    id: 1,
    title: 'Curso Básico de Computadores e Informática',
    description: 'Fundamentos tecnológicos esenciales para comprender y manejar sistemas informáticos aplicados a la industria.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2793-computacion-basica/diploma/detalle/'
  },
  {
    id: 2,
    title: 'Curso Básico de Programación con C#',
    description: 'Introducción a la programación con C# para crear soluciones orientadas a objetos en entornos industriales.',
    certificate: 'https://platzi.com/p/yefer010606/curso/3086-csharp/diploma/detalle/'
  },
  {
    id: 3,
    title: 'Curso de Programación Orientada a Objetos con C#',
    description: 'Principios de la POO aplicados en proyectos industriales robustos con C#.',
    certificate: 'https://platzi.com/p/yefer010606/curso/8036-c-sharp-poo/diploma/detalle/'
  },
  {
    id: 4,
    title: 'Curso de Fundamentos de Entity Framework',
    description: 'Gestión de bases de datos eficientes en .NET con técnicas ORM modernas.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2987-entity-framework/diploma/detalle/'
  },
  {
    id: 5,
    title: 'Curso de Fundamentos de .NET',
    description: 'Marco de desarrollo para construir aplicaciones escalables y seguras en la industria.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2883-fundamentos-net/diploma/detalle/'
  },
  {
    id: 6,
    title: 'Curso de Fundamentos de Pruebas de Software',
    description: 'Aplicación de pruebas para asegurar calidad en el ciclo de vida de productos tecnológicos.',
    certificate: 'https://platzi.com/p/yefer010606/curso/1421-pruebas-software/diploma/detalle/'
  },
  {
    id: 7,
    title: 'Curso de Desarrollo Backend con PHP',
    description: 'Construcción de servidores y lógica empresarial adaptada a sistemas industriales.',
    certificate: 'https://platzi.com/r/yefer010606/'
  },
  {
    id: 8,
    title: 'Curso de Introducción a la Web: Historia y Funcionamiento de Internet',
    description: 'Conocimientos esenciales sobre cómo funciona la web moderna en entornos industriales.',
    certificate: 'https://platzi.com/p/yefer010606/curso/7924-introweb/diploma/detalle/'
  },
  {
    id: 9,
    title: 'Curso de Pensamiento Lógico: Algoritmos y Diagramas de Flujo',
    description: 'Diseño de algoritmos eficientes para automatización y procesos industriales.',
    certificate: 'https://platzi.com/p/yefer010606/curso/3221-pensamiento-logico/diploma/detalle/'
  },
  {
    id: 10,
    title: 'Curso de Pensamiento Lógico: Lenguajes de Programación',
    description: 'Conceptos clave para entender cómo los lenguajes modelan la lógica computacional.',
    certificate: 'https://platzi.com/p/yefer010606/curso/3223-pensamiento-logico-lenguajes/diploma/detalle/'
  },
  {
    id: 11,
    title: 'Curso de Pensamiento Lógico: Manejo de Datos, Estructuras y Funciones',
    description: 'Manejo de estructuras de datos aplicadas a la eficiencia industrial.',
    certificate: 'https://platzi.com/p/yefer010606/curso/3222-pensamiento-logico-estructuras/diploma/detalle/'
  },
  {
    id: 12,
    title: 'Curso Definitivo de HTML y CSS',
    description: 'Diseño profesional de interfaces para sistemas de monitoreo industrial.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2008-html-css/diploma/detalle/'
  },
  {
    id: 13,
    title: 'Curso Práctico de HTML y CSS',
    description: 'Prácticas avanzadas para construir sitios web funcionales y responsivos.',
    certificate: 'https://platzi.com/p/yefer010606/curso/1758-html-practico/diploma/detalle/'
  },
  {
    id: 14,
    title: 'Curso de Frontend Developer',
    description: 'Desarrollo de aplicaciones modernas para visualizar datos industriales.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2467-frontend-developer/diploma/detalle/'
  },
  {
    id: 15,
    title: 'Curso Práctico de Frontend Developer',
    description: 'Construcción de aplicaciones reales con enfoque profesional.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2477-frontend-developer-practico/diploma/detalle/'
  },
  {
    id: 16,
    title: 'Curso de Flujo de Desarrollo Moderno CodeStream',
    description: 'Flujos de trabajo colaborativos para equipos de desarrollo industrial.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2157-desarrollo-moderno-codestream/diploma/detalle/'
  },
  {
    id: 17,
    title: 'Curso Profesional de Git y GitHub',
    description: 'Control de versiones y trabajo en equipo en proyectos industriales.',
    certificate: 'https://platzi.com/p/yefer010606/curso/1557-git-github/diploma/detalle/'
  },
  {
    id: 18,
    title: 'Curso Práctico de Vue.js',
    description: 'Desarrollo de interfaces dinámicas para sistemas industriales con Vue.',
    certificate: 'https://platzi.com/p/yefer010606/curso/2876-vue-practico/diploma/detalle/'
  },
  {
    id: 19,
    title: 'Curso de JavaScript',
    description: 'Lógica de programación aplicada a la automatización de tareas web.',
    certificate: 'https://platzi.com/r/yefer010606/'
  },
  {
    id: 20,
    title: 'Curso Práctico de JavaScript',
    description: 'Aplicación práctica del lenguaje en interfaces industriales inteligentes.',
    certificate: 'https://platzi.com/p/yefer010606/curso/3271-javascript-practico/diploma/detalle/'
  }
])
</script>

<template>
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" />

  <div id="Curso"  class="feature-area section-padding">
    <div class="container">
      <div class="row">
        <!-- SECCIÓN FEATURES -->
        <div class="col-lg-6 col-md-12 col-sm-12">
          <div class="section-title">
            <h6>Características Principales</h6>
            <h2>Soluciones Integrales para la Gestión y Optimización de Proyectos Industriales <b>de Alto Impacto</b></h2>
          </div>
          <div
            class="single-feature-item"
            v-for="feature in features"
            :key="feature.id"
          >
            <div class="feature-icon">
              <i :class="feature.icon"></i>
            </div>
            <div class="feature-content">
              <h5>{{ feature.title }}</h5>
              <p>{{ feature.content }}</p>
            </div>
          </div>
        </div>

        <div class="col-lg-6 col-md-12 col-sm-12">
          <div class="feature-image">
            <img src="/assets/Captura.png" alt="Imagen de proyecto industrial" />
          </div>
        </div>
      </div>

      <!-- SECCIÓN CURSOS -->
      <div class="row mt-5">
        <div class="col-12">
          <div class="section-title">
            <h6>Cursos Completados</h6>
            <h2>Estos son los cursos que he completado con <b>certificado</b></h2>
          </div>

          <div
            class="single-feature-item"
            v-for="course in courses"
            :key="course.id"
            style="margin-bottom: 1.5rem;"
          >
            <div class="feature-icon">
              <i class="fas fa-graduation-cap"></i>
            </div>
            <div class="feature-content">
              <h5>{{ course.title }}</h5>
              <p>{{ course.description }}</p>
              <a
                :href="course.certificate"
                class="btn btn-sm btn-primary mt-2"
                target="_blank"
                rel="noopener noreferrer"
              >
                Ver Certificado
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
