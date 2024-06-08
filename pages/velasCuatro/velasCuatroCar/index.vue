<template>
  <!--<v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyDetails">
    <span style="text-transform: none; color: green">
      Juicy Lemon
      Car
      9.99$
    </span>
  </v-btn>-->
  <div>
    <h2>Your Cart Item</h2>
    <p><a href="#" class="back-to-shopping">Back to shopping</a></p>
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
      <table>
        <thead>
          <tr>
            <th>Product</th>
            <th>Price</th>
            <th>Quantity</th>
            <th>Total</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(product, index) in products" :key="index">
            <td>
              <div class="product-info">
                <img src="/img/P5.png">
                <p>Juicy Lemon</p>
              </div>
            </td>
            <td>{{ product.price }}</td>
            <td>{{ product.quantity }}</td>
            <td>{{ product.price * product.quantity }}</td>
          </tr>
        </tbody>
      </table>
      <div class="subtotal-section">
        <p class="subtotal">
          Subtotal: ${{ subtotal }}
        </p>
        <button class="checkout-button" @click="VelaJuicyDetails">
          Check - out
        </button>
      </div>
    </div>

    <div><p>Tax and shipping cost will be calculate later</p></div>

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
    VelaJuicyDetails () {
      this.$router.push('/velasCuatro/velasCuatroCar/velasCuatroDetails')
    }
  }
}
</script>

<style scoped>
h2 {
  font-size: 24px;
  margin-bottom: 10px;
  text-align: center;
}

/* Estilos para el enlace "Back to shopping" */
.back-to-shopping {
  color: green;
  text-decoration: underline;
  text-align: center;
}

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

table {
  width: 100%;
  border-collapse: collapse;
}

/* Estilos para los encabezados */
th {
  background-color: #f2f2f2;
  padding: 8px;
  text-align: left;
}

/* Estilos para las celdas */
td {
  border: 1px solid #dddddd;
  padding: 8px;
}

/* Estilos para la línea negra encima y debajo de tbody */
tbody {
  border-top: 1px solid black;
  border-bottom: 1px solid black;
}

/* Estilos para la sección de subtotal */
.subtotal-section {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}

.subtotal {
  font-size: 18px;
  font-weight: bold;
}

.checkout-button {
  background-color: green;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 16px;
}

.checkout-button:hover {
  background-color: darkgreen;
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
