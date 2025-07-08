<template>
  <div class="landing-page">
    <!-- Hero Section -->
    <section class="hero">
      <div class="hero-background">
        <div class="coffee-beans"></div>
        <div class="floating-particles"></div>
      </div>

      <div class="hero-content">
        <div class="hero-logo">
          <i class="fas fa-coffee coffee-icon"></i>
          <h1 class="hero-title">Qahwa</h1>
        </div>

        <p class="hero-subtitle">El Futuro de la Producción Cafetera</p>
        <p class="hero-description">
          Conectamos a productores locales con distribuidores globales,
          revolucionando la cadena de suministro del café con tecnología de vanguardia
        </p>

        <button @click="redirigir" class="cta-button">
          <i class="fas fa-rocket"></i>
          Ir a la plataforma
        </button>

        <div class="hero-stats">
          <div class="stat">
            <span class="stat-number">500+</span>
            <span class="stat-label">Productores</span>
          </div>
          <div class="stat">
            <span class="stat-number">1000+</span>
            <span class="stat-label">Distribuidores</span>
          </div>
          <div class="stat">
            <span class="stat-number">50+</span>
            <span class="stat-label">Países</span>
          </div>
        </div>
      </div>

      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <!-- Features Section -->
    <section class="features">
      <div class="container">
        <h2 class="section-title">¿Por qué elegir Qahwa?</h2>
        <div class="features-grid">
          <div class="feature-card" v-for="feature in features" :key="feature.id">
            <div class="feature-icon">
              <i :class="feature.icon"></i>
            </div>
            <h3>{{ feature.title }}</h3>
            <p>{{ feature.description }}</p>
          </div>
        </div>
      </div>
    </section>

    <!-- How It Works Section -->
    <section class="how-it-works">
      <div class="container">
        <h2 class="section-title">¿Cómo funciona?</h2>
        <div class="steps">
          <div class="step" v-for="(step, index) in steps" :key="step.id">
            <div class="step-number">{{ index + 1 }}</div>
            <div class="step-content">
              <h3>{{ step.title }}</h3>
              <p>{{ step.description }}</p>
            </div>
            <div class="step-icon">
              <i :class="step.icon"></i>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials">
      <div class="container">
        <h2 class="section-title">Lo que dicen nuestros usuarios</h2>
        <div class="testimonials-grid">
          <div class="testimonial-card" v-for="testimonial in testimonials" :key="testimonial.id">
            <div class="testimonial-content">
              <div class="stars">
                <i class="fas fa-star" v-for="star in 5" :key="star"></i>
              </div>
              <p>"{{ testimonial.text }}"</p>
            </div>
            <div class="testimonial-author">
              <div class="author-avatar">
                <i :class="testimonial.avatar"></i>
              </div>
              <div class="author-info">
                <h4>{{ testimonial.name }}</h4>
                <span>{{ testimonial.role }}</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="final-cta">
      <div class="container">
        <h2>¿Listo para revolucionar tu negocio cafetero?</h2>
        <p>Únete a miles de productores y distribuidores que ya confían en Qahwa</p>
        <button @click="redirigir" class="cta-button large">
          <i class="fas fa-arrow-right"></i>
          Comenzar ahora
        </button>
      </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
      <div class="container">
        <div class="footer-content">
          <div class="footer-section">
            <h3><i class="fas fa-coffee"></i> Qahwa</h3>
            <p>Revolucionando el mundo del café, una conexión a la vez.</p>
          </div>
          <div class="footer-section">
            <h4>Enlaces rápidos</h4>
            <ul>
              <li><a href="#features">Características</a></li>
              <li><a href="#how-it-works">Cómo funciona</a></li>
              <li><a href="#testimonials">Testimonios</a></li>
            </ul>
          </div>
          <div class="footer-section">
            <h4>Contacto</h4>
            <p><i class="fas fa-envelope"></i> info@qahwa.com</p>
            <p><i class="fas fa-phone"></i> +51 999 999 999</p>
          </div>
        </div>
        <div class="footer-bottom">
          <p>&copy; 2025 Qahwa. Todos los derechos reservados.</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const features = ref([
  {
    id: 1,
    icon: 'fas fa-handshake',
    title: 'Conexión Directa',
    description: 'Conectamos productores y distribuidores sin intermediarios, maximizando las ganancias para ambas partes.'
  },
  {
    id: 2,
    icon: 'fas fa-leaf',
    title: 'Sostenibilidad',
    description: 'Promovemos prácticas sostenibles y comercio justo en toda la cadena de suministro del café.'
  },
  {
    id: 3,
    icon: 'fas fa-chart-line',
    title: 'Análisis en Tiempo Real',
    description: 'Herramientas avanzadas de análisis para optimizar la producción y ventas.'
  },
  {
    id: 4,
    icon: 'fas fa-shield-alt',
    title: 'Transacciones Seguras',
    description: 'Plataforma segura con pagos protegidos y garantía de calidad en cada transacción.'
  },
  {
    id: 5,
    icon: 'fas fa-globe',
    title: 'Alcance Global',
    description: 'Acceso a mercados internacionales y oportunidades de exportación.'
  },
  {
    id: 6,
    icon: 'fas fa-mobile-alt',
    title: 'Tecnología Móvil',
    description: 'Aplicación móvil intuitiva para gestionar tu negocio desde cualquier lugar.'
  }
])

const steps = ref([
  {
    id: 1,
    title: 'Registro',
    description: 'Crea tu cuenta como productor o distribuidor en minutos.',
    icon: 'fas fa-user-plus'
  },
  {
    id: 2,
    title: 'Perfil',
    description: 'Completa tu perfil con información sobre tus productos o necesidades.',
    icon: 'fas fa-edit'
  },
  {
    id: 3,
    title: 'Conexión',
    description: 'Encuentra socios comerciales ideales usando nuestro algoritmo inteligente.',
    icon: 'fas fa-search'
  },
  {
    id: 4,
    title: 'Negociación',
    description: 'Negocia precios, cantidades y términos directamente en la plataforma.',
    icon: 'fas fa-comments'
  },
  {
    id: 5,
    title: 'Transacción',
    description: 'Completa transacciones seguras con nuestro sistema de pagos integrado.',
    icon: 'fas fa-credit-card'
  }
])

const testimonials = ref([
  {
    id: 1,
    name: 'María González',
    role: 'Productora de Café - Cusco',
    avatar: 'fas fa-user-circle',
    text: 'Qahwa cambió mi vida. Ahora puedo vender directamente a distribuidores internacionales y obtener mejores precios por mi café orgánico.'
  },
  {
    id: 2,
    name: 'Roberto Silva',
    role: 'Distribuidor - Lima',
    avatar: 'fas fa-user-tie',
    text: 'La plataforma es increíble. Encontré productores de café de alta calidad y ahora mi negocio ha crecido un 300% en el último año.'
  },
  {
    id: 3,
    name: 'Ana Vargas',
    role: 'Cooperativa Cafetera - Junín',
    avatar: 'fas fa-users',
    text: 'Gracias a Qahwa, nuestra cooperativa ha logrado exportar a 5 países nuevos. La tecnología es fácil de usar y muy efectiva.'
  }
])

const redirigir = () => {
  window.location.href = 'https://qahwa-frontend.vercel.app' // Cambia por tu URL real
}

onMounted(() => {
  // Smooth scroll for navigation
  document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
      e.preventDefault()
      document.querySelector(this.getAttribute('href')).scrollIntoView({
        behavior: 'smooth'
      })
    })
  })

  // Intersection Observer for animations
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('animate-in')
      }
    })
  })

  document.querySelectorAll('.feature-card, .step, .testimonial-card').forEach(el => {
    observer.observe(el)
  })
})
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.landing-page {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  color: #333;
  overflow-x: hidden;
}

/* Hero Section */
.hero {
  height: 100vh;
  background: linear-gradient(135deg, #2c1810 0%, #4e944f 50%, #8b5e3c 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.hero-background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
}

.coffee-beans::before,
.coffee-beans::after {
  content: '☕';
  position: absolute;
  font-size: 3rem;
  color: rgba(255,255,255,0.1);
  animation: float 8s ease-in-out infinite;
}

.coffee-beans::before {
  top: 20%;
  left: 10%;
  animation-delay: 0s;
}

.coffee-beans::after {
  top: 70%;
  right: 15%;
  animation-delay: 4s;
}

.floating-particles {
  position: absolute;
  width: 100%;
  height: 100%;
  background: radial-gradient(circle, rgba(255,255,255,0.1) 1px, transparent 1px);
  background-size: 50px 50px;
  animation: drift 20s linear infinite;
}

@keyframes float {
  0%, 100% { transform: translateY(0px) rotate(0deg); }
  50% { transform: translateY(-20px) rotate(180deg); }
}

@keyframes drift {
  0% { transform: translateX(0) translateY(0); }
  100% { transform: translateX(-50px) translateY(-50px); }
}

.hero-content {
  text-align: center;
  color: white;
  z-index: 2;
  max-width: 800px;
  padding: 0 2rem;
}

.hero-logo {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  margin-bottom: 2rem;
}

.coffee-icon {
  font-size: 4rem;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.1); }
  100% { transform: scale(1); }
}

.hero-title {
  font-size: 5rem;
  font-weight: 900;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
  background: linear-gradient(45deg, #fff, #f0f0f0);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-subtitle {
  font-size: 2rem;
  margin-bottom: 1rem;
  opacity: 0.9;
  font-weight: 600;
}

.hero-description {
  font-size: 1.3rem;
  margin-bottom: 3rem;
  opacity: 0.8;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.cta-button {
  display: inline-flex;
  align-items: center;
  gap: 1rem;
  padding: 1.5rem 3rem;
  font-size: 1.3rem;
  background: linear-gradient(135deg, #fff, #f0f0f0);
  color: #4e944f;
  border: none;
  border-radius: 50px;
  cursor: pointer;
  font-weight: bold;
  text-decoration: none;
  transition: all 0.4s ease;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
  font-family: inherit;
}

.cta-button:hover {
  transform: translateY(-5px) scale(1.05);
  box-shadow: 0 15px 40px rgba(0,0,0,0.3);
  background: linear-gradient(135deg, #e6ffe6, #d4edda);
}

.cta-button.large {
  padding: 2rem 4rem;
  font-size: 1.5rem;
}

.hero-stats {
  display: flex;
  justify-content: center;
  gap: 3rem;
  margin-top: 4rem;
}

.stat {
  text-align: center;
}

.stat-number {
  display: block;
  font-size: 2.5rem;
  font-weight: 900;
  color: #fff;
}

.stat-label {
  font-size: 1rem;
  opacity: 0.8;
}

.scroll-indicator {
  position: absolute;
  bottom: 2rem;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  font-size: 1.5rem;
  animation: bounce 2s infinite;
}

@keyframes bounce {
  0%, 20%, 50%, 80%, 100% { transform: translateX(-50%) translateY(0); }
  40% { transform: translateX(-50%) translateY(-10px); }
  60% { transform: translateX(-50%) translateY(-5px); }
}

/* Container */
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

/* Section Title */
.section-title {
  text-align: center;
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 3rem;
  color: #2c1810;
  position: relative;
}

.section-title::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 100px;
  height: 4px;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  border-radius: 2px;
}

/* Features Section */
.features {
  padding: 6rem 0;
  background: linear-gradient(135deg, #f8f9fa, #e9ecef);
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.feature-card {
  background: white;
  padding: 2.5rem;
  border-radius: 20px;
  text-align: center;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1);
  transition: all 0.3s ease;
  opacity: 0;
  transform: translateY(30px);
}

.feature-card.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.feature-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 20px 40px rgba(0,0,0,0.15);
}

.feature-icon {
  width: 80px;
  height: 80px;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto 1.5rem;
  font-size: 2rem;
  color: white;
}

.feature-card h3 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #2c1810;
}

.feature-card p {
  color: #666;
  line-height: 1.6;
}

/* How It Works Section */
.how-it-works {
  padding: 6rem 0;
  background: white;
}

.steps {
  display: flex;
  flex-direction: column;
  gap: 3rem;
}

.step {
  display: flex;
  align-items: center;
  gap: 2rem;
  opacity: 0;
  transform: translateX(-30px);
  transition: all 0.6s ease;
}

.step.animate-in {
  opacity: 1;
  transform: translateX(0);
}

.step:nth-child(even) {
  flex-direction: row-reverse;
}

.step:nth-child(even) .step-content {
  text-align: right;
}

.step-number {
  width: 80px;
  height: 80px;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  font-weight: 900;
  color: white;
  flex-shrink: 0;
}

.step-content {
  flex: 1;
}

.step-content h3 {
  font-size: 1.8rem;
  margin-bottom: 1rem;
  color: #2c1810;
}

.step-content p {
  color: #666;
  font-size: 1.1rem;
  line-height: 1.6;
}

.step-icon {
  width: 60px;
  height: 60px;
  background: linear-gradient(135deg, #f8f9fa, #e9ecef);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.5rem;
  color: #4e944f;
  flex-shrink: 0;
}

/* Testimonials Section */
.testimonials {
  padding: 6rem 0;
  background: linear-gradient(135deg, #2c1810, #4e944f);
  color: white;
}

.testimonials .section-title {
  color: white;
}

.testimonials-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.testimonial-card {
  background: rgba(255,255,255,0.1);
  padding: 2rem;
  border-radius: 20px;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255,255,255,0.2);
  transition: all 0.3s ease;
  opacity: 0;
  transform: translateY(30px);
}

.testimonial-card.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.testimonial-card:hover {
  transform: translateY(-5px);
  background: rgba(255,255,255,0.15);
}

.stars {
  color: #ffd700;
  margin-bottom: 1rem;
  font-size: 1.2rem;
}

.testimonial-content p {
  font-size: 1.1rem;
  line-height: 1.6;
  margin-bottom: 1.5rem;
  font-style: italic;
}

.testimonial-author {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.author-avatar {
  width: 50px;
  height: 50px;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.5rem;
  color: white;
}

.author-info h4 {
  margin-bottom: 0.25rem;
  font-size: 1.1rem;
}

.author-info span {
  opacity: 0.8;
  font-size: 0.9rem;
}

/* Final CTA Section */
.final-cta {
  padding: 6rem 0;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  text-align: center;
  color: white;
}

.final-cta h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  font-weight: 700;
}

.final-cta p {
  font-size: 1.3rem;
  margin-bottom: 3rem;
  opacity: 0.9;
}

/* Footer */
.footer {
  background: #2c1810;
  color: white;
  padding: 3rem 0 1rem;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin-bottom: 2rem;
}

.footer-section h3 {
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.footer-section h4 {
  margin-bottom: 1rem;
  color: #4e944f;
}

.footer-section ul {
  list-style: none;
}

.footer-section ul li {
  margin-bottom: 0.5rem;
}

.footer-section a {
  color: #ccc;
  text-decoration: none;
  transition: color 0.3s ease;
}

.footer-section a:hover {
  color: #4e944f;
}

.footer-section p {
  margin-bottom: 0.5rem;
  color: #ccc;
}

.footer-bottom {
  text-align: center;
  padding-top: 2rem;
  border-top: 1px solid #444;
  color: #999;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-title {
    font-size: 3rem;
  }

  .hero-subtitle {
    font-size: 1.5rem;
  }

  .hero-description {
    font-size: 1.1rem;
  }

  .hero-stats {
    flex-direction: column;
    gap: 1rem;
  }

  .section-title {
    font-size: 2rem;
  }

  .features-grid {
    grid-template-columns: 1fr;
  }

  .step {
    flex-direction: column !important;
    text-align: center;
  }

  .step-content {
    text-align: center !important;
  }

  .testimonials-grid {
    grid-template-columns: 1fr;
  }

  .final-cta h2 {
    font-size: 2rem;
  }
}

@media (max-width: 480px) {
  .hero-content {
    padding: 0 1rem;
  }

  .hero-logo {
    flex-direction: column;
    gap: 0.5rem;
  }

  .hero-title {
    font-size: 2.5rem;
  }

  .cta-button {
    padding: 1rem 2rem;
    font-size: 1.1rem;
  }

  .feature-card,
  .testimonial-card {
    padding: 1.5rem;
  }

  .container {
    padding: 0 1rem;
  }
}
</style>