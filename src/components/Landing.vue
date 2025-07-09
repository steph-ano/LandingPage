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

        <button class="cta-button" @click="redirigir">
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

    <!-- Product Video Section -->
    <section class="video-section product">
      <div class="container">
        <h2 class="section-title">Conoce Nuestra Plataforma</h2>
        <div class="video-content">
          <div class="video-info">
            <h3>Innovación en Cada Función</h3>
            <p>
              Descubre cómo Qahwa está transformando la industria del café con tecnología de vanguardia.
              Nuestra plataforma integra inteligencia artificial, análisis de mercado en tiempo real y
              herramientas de gestión avanzadas para optimizar cada aspecto de tu negocio cafetero.
            </p>
            <ul class="video-highlights">
              <li><i class="fas fa-check"></i> Matching inteligente entre productores y distribuidores</li>
              <li><i class="fas fa-check"></i> Análisis predictivo de precios y tendencias</li>
              <li><i class="fas fa-check"></i> Gestión automatizada de inventarios</li>
              <li><i class="fas fa-check"></i> Trazabilidad completa del producto</li>
            </ul>
          </div>
          <div class="video-container">
            <div class="video-wrapper">
              <div class="video-responsive">
                <iframe
                    src="https://www.youtube.com/embed/epva2WCBLI8"
                    title="Demo del Producto"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                    allowfullscreen>
                </iframe>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="features">
      <div class="container">
        <h2 class="section-title">¿Por qué elegir Qahwa?</h2>
        <div class="features-grid">
          <div class="feature-card">
            <div class="feature-icon">
              <i class="fas fa-handshake"></i>
            </div>
            <h3>Conexión Directa</h3>
            <p>Conectamos productores y distribuidores sin intermediarios, maximizando las ganancias para ambas partes.</p>
          </div>
          <div class="feature-card">
            <div class="feature-icon">
              <i class="fas fa-leaf"></i>
            </div>
            <h3>Sostenibilidad</h3>
            <p>Promovemos prácticas sostenibles y comercio justo en toda la cadena de suministro del café.</p>
          </div>
          <div class="feature-card">
            <div class="feature-icon">
              <i class="fas fa-chart-line"></i>
            </div>
            <h3>Análisis en Tiempo Real</h3>
            <p>Herramientas avanzadas de análisis para optimizar la producción y ventas.</p>
          </div>
          <div class="feature-card">
            <div class="feature-icon">
              <i class="fas fa-shield-alt"></i>
            </div>
            <h3>Transacciones Seguras</h3>
            <p>Plataforma segura con pagos protegidos y garantía de calidad en cada transacción.</p>
          </div>
          <div class="feature-card">
            <div class="feature-icon">
              <i class="fas fa-globe"></i>
            </div>
            <h3>Alcance Global</h3>
            <p>Acceso a mercados internacionales y oportunidades de exportación.</p>
          </div>
          <div class="feature-card">
            <div class="feature-icon">
              <i class="fas fa-mobile-alt"></i>
            </div>
            <h3>Tecnología Móvil</h3>
            <p>Aplicación móvil intuitiva para gestionar tu negocio desde cualquier lugar.</p>
          </div>
        </div>
      </div>
    </section>
    <section class="how-it-works">
      <div class="container">
        <h2 class="section-title">¿Cómo funciona?</h2>
        <div class="steps">
          <div class="step">
            <div class="step-number">1</div>
            <div class="step-content">
              <h3>Registro</h3>
              <p>Crea tu cuenta como productor o distribuidor en minutos.</p>
            </div>
            <div class="step-icon">
              <i class="fas fa-user-plus"></i>
            </div>
          </div>
          <div class="step">
            <div class="step-number">2</div>
            <div class="step-content">
              <h3>Perfil</h3>
              <p>Completa tu perfil con información sobre tus productos o necesidades.</p>
            </div>
            <div class="step-icon">
              <i class="fas fa-edit"></i>
            </div>
          </div>
          <div class="step">
            <div class="step-number">3</div>
            <div class="step-content">
              <h3>Conexión</h3>
              <p>Encuentra socios comerciales ideales usando nuestro algoritmo inteligente.</p>
            </div>
            <div class="step-icon">
              <i class="fas fa-search"></i>
            </div>
          </div>
          <div class="step">
            <div class="step-number">4</div>
            <div class="step-content">
              <h3>Negociación</h3>
              <p>Negocia precios, cantidades y términos directamente en la plataforma.</p>
            </div>
            <div class="step-icon">
              <i class="fas fa-comments"></i>
            </div>
          </div>
          <div class="step">
            <div class="step-number">5</div>
            <div class="step-content">
              <h3>Transacción</h3>
              <p>Completa transacciones seguras con nuestro sistema de pagos integrado.</p>
            </div>
            <div class="step-icon">
              <i class="fas fa-credit-card"></i>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="video-section team">
      <div class="container">
        <h2 class="section-title">Conoce a Nuestro Equipo</h2>
        <div class="video-content">
          <div class="video-info animate-in">
            <h3>Pasión por el Café, Experiencia en Tecnología</h3>
            <p>
              Nuestro equipo multidisciplinario combina décadas de experiencia en la industria del café
              con conocimiento tecnológico de vanguardia. Desde ingenieros de software hasta expertos
              en comercio internacional, todos comparten una misma pasión: transformar el sector cafetero.
            </p>
            <ul class="video-highlights">
              <li><i class="fas fa-check"></i> 15+ años de experiencia en agroindustria</li>
              <li><i class="fas fa-check"></i> Especialistas en desarrollo de software</li>
              <li><i class="fas fa-check"></i> Expertos en comercio internacional</li>
              <li><i class="fas fa-check"></i> Consultores en sostenibilidad</li>
            </ul>
          </div>
          <div class="video-container animate-in">
            <div class="video-wrapper">
              <div class="video-responsive">
                <iframe
                    src="https://www.youtube.com/embed/TzVDiXxyA2A"
                    title="Presentación del Equipo"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                    allowfullscreen>
                </iframe>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="testimonials">
      <div class="container">
        <h2 class="section-title">Lo que dicen nuestros usuarios</h2>
        <div class="testimonials-grid">
          <div class="testimonial-card">
            <div class="testimonial-content">
              <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
              </div>
              <p>"Qahwa cambió mi vida. Ahora puedo vender directamente a distribuidores internacionales y obtener mejores precios por mi café orgánico."</p>
            </div>
            <div class="testimonial-author">
              <div class="author-avatar">
                <i class="fas fa-user-circle"></i>
              </div>
              <div class="author-info">
                <h4>María González</h4>
                <span>Productora de Café - Cusco</span>
              </div>
            </div>
          </div>
          <div class="testimonial-card">
            <div class="testimonial-content">
              <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
              </div>
              <p>"La plataforma es increíble. Encontré productores de café de alta calidad y ahora mi negocio ha crecido un 300% en el último año."</p>
            </div>
            <div class="testimonial-author">
              <div class="author-avatar">
                <i class="fas fa-user-tie"></i>
              </div>
              <div class="author-info">
                <h4>Roberto Silva</h4>
                <span>Distribuidor - Lima</span>
              </div>
            </div>
          </div>
          <div class="testimonial-card">
            <div class="testimonial-content">
              <div class="stars">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
              </div>
              <p>"Gracias a Qahwa, nuestra cooperativa ha logrado exportar a 5 países nuevos. La tecnología es fácil de usar y muy efectiva."</p>
            </div>
            <div class="testimonial-author">
              <div class="author-avatar">
                <i class="fas fa-users"></i>
              </div>
              <div class="author-info">
                <h4>Ana Vargas</h4>
                <span>Cooperativa Cafetera - Junín</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="final-cta">
      <div class="container">
        <h2>¿Listo para revolucionar tu negocio cafetero?</h2>
        <p>Únete a miles de productores y distribuidores que ya confían en Qahwa</p>
        <button class="cta-button large" onclick="redirigir()">
          <i class="fas fa-arrow-right"></i>
          Comenzar ahora
        </button>
      </div>
    </section>
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
    <!-- Aquí puedes seguir agregando las demás secciones de la landing page como <section class="features">, etc. -->
  </div>
</template>

<script>
export default {
  name: 'LandingPage',
  mounted() {
    // Animaciones
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('animate-in');
        }
      });
    }, {
      threshold: 0.1,
      rootMargin: '0px 0px -50px 0px'
    });

    document.querySelectorAll('.feature-card, .step, .testimonial-card, .video-info, .video-container')
        .forEach(el => observer.observe(el));
  },
  methods: {
    redirigir() {
      window.location.href = 'https://qahwa-frontend.vercel.app';
    },
    mostrarAlerta(tipo) {
      alert(`Aquí se reproduciría el video: ${tipo}`);
    }
  }
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
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

/* Video Sections */
.video-section {
  padding: 6rem 0;
  position: relative;
}

.video-section.product {
  background: linear-gradient(135deg, #f8f9fa, #e9ecef);
}

.video-section.team {
  background: white;
}

.video-section .section-title.white {
  color: white;
}

.video-section.team {
  background: linear-gradient(135deg, #2c1810, #4e944f);
  color: white;
}

.video-section.team .section-title {
  color: white;
}

.video-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}

.video-info {
  opacity: 0;
  transform: translateX(-50px);
  transition: all 0.8s ease;
}

.video-info.animate-in {
  opacity: 1;
  transform: translateX(0);
}

.video-info h3 {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
  font-weight: 700;
  color: #2c1810;
}

.video-section.team .video-info h3 {
  color: white;
}

.video-info p {
  font-size: 1.2rem;
  line-height: 1.8;
  margin-bottom: 1.5rem;
  opacity: 0.9;
}

.video-highlights {
  list-style: none;
  margin-top: 2rem;
}

.video-highlights li {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

.video-highlights li i {
  width: 25px;
  height: 25px;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 0.8rem;
  flex-shrink: 0;
}

.video-container {
  position: relative;
  opacity: 0;
  transform: translateY(50px);
  transition: all 0.8s ease;
}

.video-container.animate-in {
  opacity: 1;
  transform: translateY(0);
}

.video-wrapper {
  position: relative;
  background: linear-gradient(135deg, #4e944f, #8b5e3c);
  border-radius: 20px;
  padding: 1.5rem;
  box-shadow: 0 20px 60px rgba(0,0,0,0.2);
}

.video-placeholder {
  width: 100%;
  height: 300px;
  background: linear-gradient(135deg, #2c1810, #4e944f);
  border-radius: 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 1.2rem;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.video-placeholder::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(45deg, transparent 40%, rgba(255,255,255,0.1) 50%, transparent 60%);
  animation: shine 3s ease-in-out infinite;
}

@keyframes shine {
  0% { transform: translateX(-100%); }
  100% { transform: translateX(100%); }
}

.play-button {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 80px;
  height: 80px;
  background: rgba(255,255,255,0.9);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 10px 30px rgba(0,0,0,0.2);
}

.play-button:hover {
  transform: translate(-50%, -50%) scale(1.1);
  background: white;
}

.play-button i {
  font-size: 2rem;
  color: #4e944f;
  margin-left: 5px;
}

.video-badge {
  position: absolute;
  top: 1rem;
  right: 1rem;
  background: rgba(255,255,255,0.9);
  color: #4e944f;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  font-weight: 600;
  display: flex;
  align-items: center;
  gap: 0.5rem;
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

  .video-content {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .video-info h3 {
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

  .video-placeholder {
    height: 200px;
  }
}
.video-responsive {
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
  overflow: hidden;
  border-radius: 12px;
}

.video-responsive iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>