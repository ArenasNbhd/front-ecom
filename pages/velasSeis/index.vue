<template>
  <!--<v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantCar">
    <span style="text-transform: none; color: green">
      Fragant View
    </span>
  </v-btn>-->
  <div>
    <v-app-bar class="top-card">
      <img src="@/img/logo.png" alt="Logo" height="40px" style="margin-right: 10px;">
      <v-toolbar-title>Candleaf</v-toolbar-title>
      <v-spacer />
      <div class="middle-titles">
        <div>Discover</div>
        <div>About</div>
        <div>Contact us</div>
      </div>
      <v-spacer />
      <v-toolbar-items>
        <v-btn icon color="black" @click="showSignup = true">
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

    <div>
      <div class="container">
        <div class="left-side">
          <img src="@/img/P6.png" class="CenteredImg">
          <div class="text-box">
            <p>All hand-made with natural soy wax, Candeleaf is made for you pleasure moments</p>
            <p style="color: green;">
              🚚 FREE SHIPPING
            </p>
          </div>
        </div>
        <div class="right-side">
          <p>Fragrant Cinammon Candleaf</p>
          <p style="color: green;">
            $9.99
          </p>
          <div class="option1">
            <label><input type="radio" name="option" value="option"> One time Purchase</label>
          </div>
          <div class="option2">
            <label><input type="radio" name="option" value="option"> Suscribe and deleviry every </label>
            <p>
              Suscribe now and get the 10% of discount on every recurring order. This discount will
              be applied at check out
            </p>
            <p style="color: green;">
              see details
            </p>
          </div>
          <v-btn color="Green" elevation="0" block @click="VelaFragantCar">
            <span style="text-transform: none; color: green">
              + Add to cart
            </span>
          </v-btn>
          <div>
            <p>Wax: Top grade. Soy wax that delivery a smoke less, consistent burn</p>
            <p>Fragance: Premium Quiality ingredients with natural essecial oils</p>
            <p>Burning time: 70-75 hours  Dimension: 10cm x 5 cm  Weight: 400 g</p>
          </div>
        </div>
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

<script>
export default {
  methods: {
    VelaFragantCar () {
      this.$router.push('/velasSeis/velasSeisCar')
    }
  }
}
</script>

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

.container {
  display: flex;
}

.text-box {
  margin-top: 10px;
  text-align: center;
}

.add-cart-btn {
  margin-top: 20px;
  background-color: green;
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
}

.left-side {
  flex: 1;
  background-color: #f0f0f0; /* Color de fondo de la parte izquierda */
  display: flex;
  justify-content: center;
  align-items: center;
}

.centeredImg {
  max-width: 100%;
  max-height: 100%;
}

.right-side {
  flex: 1;
  background-color: white; /* Color de fondo de la parte derecha */
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
