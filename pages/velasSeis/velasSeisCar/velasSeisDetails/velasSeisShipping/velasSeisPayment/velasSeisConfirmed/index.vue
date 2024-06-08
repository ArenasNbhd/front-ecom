<template>
  <!--<v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantReturn">
    <span style="text-transform: none; color: green">
      Return
    </span>
  </v-btn>-->
  <div class="container">
    <div class="left-side">
      <div class="title">
        <img src="@/img/logo.png" class="logo">
        <h2 style="color: green;">
          Candleft
        </h2>
      </div>
      <div class="nav">
        <p style="color: green;">
          Cart
        </p>
        <p style="color: green">
          >  Details
        </p>
        <p style="color: green;">
          > Shipping
        </p>
        <p style="color: black;">
          >  Payment
        </p>
      </div>

      <div class="containerS">
        <img src="@/img/Check.png" class="imagen2">

        <div>
          <h2>Payment Confirmed</h2>
        </div>

        <div>
          <p style="color: green;">
            ORDER #2039 <!--Intentar que sean numero aleatorios-->
          </p>
        </div>

        <div>
          <p style="color: gray">
            Thank you (usuario) for buying Candleaf. The nature is grateful to you.
            Now that your order is confirmed it will be ready to ship in 2 days.
            Please check your inbox in the future for you order updates.
          </p>
        </div>

        <div class="finalcontainer">
          <span class="back-to-cart">Print receipt</span>
        </div>
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantReturn">
          <span style="text-transform: none; color: green">
            Back to shopping
          </span>
        </v-btn>
      </div>
    </div>

    <div class="right-side">
      <div class="container2">
        <img src="@/img/P6.png" alt="" class="imagen">
        <div class="Info">
          <p>Fragrant Cinammon Candleaf</p>
          <p style="color: green;">
            $9.99
          </p>
        </div>
      </div>

      <div class="contact">
        <p>Subtotal</p>
        <p>$9.99</p>
      </div>

      <div class="contact">
        <p>Shipping</p>
        <p>Calculate at the next step</p>
      </div>

      <div class="contact">
        <p style="color: green;">
          Total
        </p>
        <h2 style="color: green;">
          $9.99
        </h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    VelaFragantReturn () {
      this.$router.push('/')
    }
  }
}
</script>

<style scoped>
.container {
  display: flex;
  height: 100vh; /* Altura de toda la ventana */
}

.containerS{
  justify-content: center;
  align-items: center;
  text-align: center;
}

.left-side, .right-side {
  flex: 1; /* Cada parte ocupa la mitad del ancho */
  padding: 20px;
}

.left-side {
  background-color: white; /* Color de fondo para la parte izquierda */
}

.right-side {
  background-color: #f0f0f0; /* Color de fondo para la parte derecha */
}

.logo {
  max-width: 10%;
  height: auto;
  margin-right: 10px;
}

.title {
  display: flex;
    align-items: center;
}

.nav {
  display: flex;
    align-items: center;
    justify-content: flex-start;
}

.nav > *:not(:last-child) {
  margin-right: 10px; /* Ajusta el espacio entre los elementos (puedes ajustar el valor según sea necesario) */
}

.contact {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

input {
  width: calc(100% - 8px); /* Ancho del input menos el ancho de los bordes */
  border: none; /* Elimina el borde predeterminado */
  padding: 6px; /* Espaciado dentro del input */
}

.boton {
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

input[type="checkbox"] {
  margin-right: 1px; /* Espacio entre el cuadro y el texto */
}

label {
  display: flex;
  align-items: center; /* Centra verticalmente */
  justify-content: space-between;
}

h1 {
  font-size: 14px; /* Tamaño de fuente más pequeño para "Free" */
  margin-left: auto;
}

.finalcontainer {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.back-to-cart {
  text-decoration: underline;
  margin-right: 10px; /* Ajusta el margen entre el texto y el botón según lo necesites */
}

.go-to-shipping {
  background-color: green;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
}

.container2 {
  display: flex;
  align-items: center;
}

.imagen {
  width: 350px; /* Tamaño del logo */
  margin-right: 10px;
}

.imagen2 {
  width: 150px; /* Tamaño del logo */
  margin-right: 10px;
}

.textos {
  margin-left: 10px; /* Ajusta el margen izquierdo según sea necesario */
}

input[type="text2"] {
  width: 75%; /* Ajusta el ancho del cuadro de texto al 100% */
  background-color: white; /* Fondo blanco */
  border: 2px solid #999; /* Contorno gris */
  padding: 8px; /* Espaciado interno */
  border-radius: 4px; /* Bordes redondeados */
}

button {
  width: 25%; /* Ajusta el ancho del botón al 100% */
  background-color: #ccc; /* Color de fondo gris */
  border: none; /* Sin borde */
  padding: 8px 12px; /* Espaciado interno */
  cursor: pointer; /* Cambia el cursor al pasar por encima */
  outline: none; /* Quita el contorno al hacer clic */
}

button:hover {
  background-color: #999; /* Cambia el color de fondo al pasar el cursor sobre el botón */
}

</style>
