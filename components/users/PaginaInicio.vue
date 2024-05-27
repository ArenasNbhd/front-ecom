<template>
  <div>
    <!-- Barra de Navegación -->
    <v-app-bar class="top-card">
      <img src="@/img/logo.png" alt="Logo" height="40px" style="margin-right: 10px;">
      <v-toolbar-title>Candleaf</v-toolbar-title>
      <div class="middle-titles">
        <div>Discover</div>
        <div>About</div>
        <div>Contact us</div>
      </div>
      <v-spacer />
      <v-toolbar-items>
        <v-btn icon color="black">
          <v-icon>
            mdi-account
          </v-icon>
        </v-btn>
        <v-btn icon color="black">
          <v-icon>
            mdi-cart
          </v-icon>
        </v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <!-- Cuadro de información -->
    <div class="info-box">
      <img src="@/img/plantita.jpg" alt="Imagen" style="width: 50px; margin-bottom: 10px;">
      <p class="logo-text">
        The Nature Candle
      </p>
      <p>All handmade with natural soy wax, Candleaf is a companion for all your pleasure moments.</p>
      <div style="background-color: green; color: white; padding: 10px; text-align: center; margin-top: 20px;">
        Discover our collection
      </div>
    </div>

    <!-- Nuevo div para los cuadros -->
    <div class="ProductosHeader">
      <p class="logo-text">
        Products
      </p>
      <p>Order it for you or for your beloved ones</p>
    </div>
    <div class="image-grid">
      <div class="grid-item">
        <img src="@/img/P1.png" alt="Imagen 1">
        <p>Spiced Mint</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P2.png" alt="Imagen 2">
        <p>Sweer Straweberry</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P3.png" alt="Imagen 2">
        <p>Cool Blueberries</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P4.png" alt="Imagen 1">
        <p>Juicy Lemon</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P5.png" alt="Imagen 2">
        <p>Stary Golden</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P6.png" alt="Imagen 2">
        <p>Fragrant Cinnamon</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P7.png" alt="Imagen 2">
        <p>Sumemer Cherries</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P8.png" alt="Imagen 2">
        <p>Clean Lavander</p>
      </div>
      <!-- Repite estos divs si quieres agregar mas productos -->
    </div>
    <!-- Nuevo div Informacion en dos partes -->
    <div class="split-container">
      <div class="left-side">
        <p class="logo-text">
          Clean and fragrant soy wax
        </p>
        <p>Made for your home and for your wellness</p>
        <p>✔ Eco-sustainable: All recyclable materials, 0% CO2 emissions</p>
        <p>✔ Hypoallergenic: 100% natural, human-friendly ingredients</p>
        <p>✔ Handmade: All candles are craftly made with love</p>
        <p>✔ Long burning: No more waste. Created to last long</p>
        <div class="learn-more">
          Learn more
        </div>
      </div>
      <div class="right-side">
        <img src="@/img/DuoV.png" alt="Imagen" class="right-image">
      </div>
    </div>

    <!-- Nuevo div para testimonios -->
    <div class="testimonials-container">
      <div class="testimonials-header">
        <p class="logo-text">
          Testimonials
        </p>
        <p>Some quotes from our happy customers</p>
      </div>
      <div class="testimonials-grid">
        <div class="testimonial-item">
          <img src="@/img/T4.jpg" alt="Testimonio 1" class="testimonial-image">
          <div class="stars">
            ★★★★★
          </div>
          <p>"I love it! No more air fresheners"</p>
          <p>Luisa</p>
        </div>
        <div class="testimonial-item">
          <img src="@/img/T2.jpg" alt="Testimonio 2" class="testimonial-image">
          <div class="stars">
            ★★★★★
          </div>
          <p>"Raccomended for everyone"</p>
          <p>Eduardo</p>
        </div>
        <div class="testimonial-item">
          <img src="@/img/T3.jpg" alt="Testimonio 3" class="testimonial-image">
          <div class="stars">
            ★★★★★
          </div>
          <p>"Looks very natural, the smell is awesome"</p>
          <p>Mart</p>
        </div>
      </div>
    </div>

    <!-- Nuevo div para lo mas comprado -->
    <div class="ProductosHeader">
      <p class="logo-text">
        Popular
      </p>
      <p>Our top selling productos that you may like</p>
    </div>
    <div class="image-grid">
      <div class="grid-item">
        <img src="@/img/P1.png" alt="Imagen 1">
        <p>Spiced Mint</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P2.png" alt="Imagen 2">
        <p>Sweer Straweberry</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P3.png" alt="Imagen 2">
        <p>Cool Blueberries</p>
      </div>
      <div class="grid-item">
        <img src="@/img/P4.png" alt="Imagen 1">
        <p>Juicy Lemon</p>
      </div>
    </div>
    <!-- Div final de la página -->
    <div class="final-container">
      <!-- Línea blanca -->
      <div class="line" />

      <!-- Contenido principal -->
      <div class="content">
        <!-- Logo y texto -->
        <div class="logo">
          <img src="@/img/logo.png" alt="Candleaf" class="logo-image">
          <p class="logo-text">
            Candleaf
          </p>
        </div>
      </div>
      <div>
        <p>Your natural candle made for your home and for your wellness</p>
      </div>
      <!-- Columnas -->
      <div class="columns">
        <!-- Columna 1 -->
        <div class="column">
          <p class="green-text">
            <strong>Discovery</strong>
          </p>
          <p>New season</p>
          <p>Most searched</p>
          <p>Most sold</p>
        </div>

        <!-- Columna 2 -->
        <div class="column">
          <p class="green-text">
            <strong>About</strong>
          </p>
          <p>Help</p>
          <p>Shipping</p>
          <p>Affiliate</p>
        </div>

        <!-- Columna 3 -->
        <div class="column">
          <p class="green-text">
            <strong>Info</strong>
          </p>
          <p>Contact us</p>
          <p>Privacy policies</p>
          <p>Terms & conditions</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.top-card {
  position: fixed;
  top: 0;
  width: 100%; /* Asegura que ocupe todo el ancho */
  z-index: 999; /* Asegura que esté por encima de otros elementos */
}

.middle-titles {
  display: flex;
  align-items: center;
  flex-grow: 1;
  margin: 0 20px;
  justify-content: center;
}

.middle-titles div {
  margin: 0 10px;
}

.middle-titles div:not(:last-child) {
  margin-right: 30px;
}

.info-box {
  background-color: white;
  padding: 60px;
  text-align: center;
  margin: 20px auto; /* Centra horizontalmente */
  width: 60%; /* Ancho del cuadro de información */
}

.ProductosHeader {
  text-align: center;
  margin: 20px auto; /* Centra el div horizontalmente */
}

.image-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* Crea 4 columnas */
  grid-gap: 50px; /* Espacio entre los elementos */
}

.grid-item {
  text-align: center;
}

.grid-item img {
  width: 100%;
  height: auto;
}

.split-container {
  display: flex;
  justify-content: space-between;
  margin: 20px auto;
  width: 100%; /* Ajusta el contenedor para que ocupe el ancho completo */
  padding: 0 20px; /* Opcional: agrega un poco de espacio a los lados */
  box-sizing: border-box; /* Incluye el padding dentro del ancho total */
}

.left-side {
  flex: 1;
  padding: 20px;
}

.right-side {
  flex: 1;
  display: flex;
  justify-content: center; /* Centra la imagen horizontalmente */
  align-items: center; /* Centra la imagen verticalmente */
  padding: 20px;
}

.right-image {
  max-width: 100%;
  height: auto;
}

.learn-more {
  background-color: green;
  color: white;
  padding: 10px;
  text-align: center;
  margin-top: 20px;
  display: inline-block;
}

.testimonials-container {
  text-align: center;
  margin: 40px auto;
}

.testimonials-header p {
  margin: 5px 0;
}

.testimonials-grid {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.testimonial-item {
  background-color: white;
  border: 1px solid #ddd;
  padding: 20px;
  margin: 0 10px;
  text-align: center;
  width: 30%;
  box-sizing: border-box;
}

.testimonial-image {
  width: 100px; /* Tamaño de la imagen */
  height: 100px; /* Tamaño de la imagen */
  border-radius: 50%; /* Hace que la imagen sea circular */
  margin-bottom: 10px;
}

.stars {
  color: green;
  font-size: 20px;
}

.final-container {
  background-color: #f0f0f0; /* Gris claro */
  padding: 20px;
}

.logo-text {
  font-size: 24px; /* Tamaño de la fuente */
  font-weight: bold; /* Negrita */
  margin: 0; /* Elimina el margen predeterminado del párrafo */
}

.line {
  border-top: 5px solid white; /* Línea blanca */
  margin-bottom: 20px; /* Espacio después de la línea */
}

.content {
  display: flex;
  align-items: center;
}

.logo {
  display: flex;
  align-items: center;
}

.logo-image {
  width: 50px; /* Tamaño del logo */
  margin-right: 10px; /* Espacio entre el logo y el texto */
}

.green-text {
  color: green; /* Color verde */
}

.columns {
  display: flex;
}

.column {
  flex: 1;
}
</style>
