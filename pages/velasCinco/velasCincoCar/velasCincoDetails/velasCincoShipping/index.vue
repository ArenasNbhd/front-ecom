<template>
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
        <p style="color: black;">
          > Shipping
        </p>
        <p style="color: gray;">
          >  Payment
        </p>
      </div>

      <div class="cuadro">
        <div class="parte-izquierda">
          Contact
        </div>
        <div class="parte-centro">
          <input type="text" placeholder="Escribe tu usuario por favor">
        </div>
        <div class="parte-derecha">
          <a href="#" class="edit-link">Edit</a>
        </div>
      </div>

      <div class="cuadro">
        <div class="parte-izquierda">
          ship to
        </div>
        <div class="parte-centro">
          <input type="text" placeholder="Escribe tu direccion por favor">
        </div>
        <div class="parte-derecha">
          <a href="#" class="edit-link">Edit</a>
        </div>
      </div>

      <div>
        <h2>Shipping method</h2>
      </div>

      <div class="cuadro3">
        <label><input type="radio" name="option" value="option"></label>
        <p>Standar Shipping</p>
        <h1>Free</h1>
      </div>

      <div class="finalcontainer">
        <span class="back-to-cart">Back to details</span>
      </div>
      <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryPayment">
        <span style="text-transform: none; color: green">
          Go to Payment
        </span>
      </v-btn>
    </div>

    <div class="right-side">
      <div class="container2">
        <img src="@/img/P5.png" alt="" class="imagen">
        <div class="Info">
          <p>Spiced Mint Candleaf</p>
          <p style="color: green;">
            $9.99
          </p>
        </div>
      </div>
      <div class="cupon-code">
        <input type="text2" placeholder="Cupon Code">
        <button class="add-code">
          Add Code
        </button>
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
        <p>Total</p>
        <h2>$9.99</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    VelaStaryPayment () {
      this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails/velasCincoShipping/velasCincoPayment')
    }
  }
}
</script>

<style scoped>
.container {
  display: flex;
  height: 100vh; /* Altura de toda la ventana */
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

.cuadro {
  border: 1px solid green; /* Contorno verde */
  width: 100%; /* Ancho igual al del div principal */
  display: flex;
}

.parte-izquierda, .parte-centro, .parte-derecha {
    flex: 1;
}

.parte-izquierda {
    background-color: white; /* solo para visualización */
    margin: 0 10px;
    flex: 0.2; /* Cambiar el tamaño */
}

.parte-centro {
    background-color: white; /* solo para visualización */
    margin: 0 10px;
    flex: 0.6; /* Cambiar el tamaño */
}

.parte-derecha {
    background-color: white; /* solo para visualización */
    text-align: center;
    margin: 0 10px;
    flex: 0.2; /* Cambiar el tamaño */
}

.edit-link {
    color: green;
    text-decoration: underline;
    cursor: pointer;
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

.cuadro3 {
  display: flex;
  align-items: center; /* Centra verticalmente */
  gap: 10px; /* Espacio entre elementos */
  padding: 10px; /* Espacio interno */
  border: 1px solid green;
}

label {
  display: flex;
  align-items: center; /* Centra verticalmente */
  justify-content: space-between;
}

input[type="radio"] {
  /* Estilos para hacer el botón circular */
  width: 20px;
  height: 20px;
  border-radius: 50%;
}

h1 {
  font-size: 14px; /* Tamaño de fuente más pequeño para "Free" */
  margin-left: auto;
}

.cuadro2 {
  border: 1px solid green;
  display: flex; /* Utiliza flexbox para alinear los elementos horizontalmente */
}

.cuadro2 input[type="text"] {
  flex: 1; /* Distribuye el espacio disponible entre los elementos */
  margin-right: 5px; /* Ajusta el espacio entre los cuadros de texto */
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

.textos {
  margin-left: 10px; /* Ajusta el margen izquierdo según sea necesario */
}

.cupon-code, .add-code {
  flex: 1; /* Establece que ocupen 1/4 del espacio cada uno */
  margin-left: 10px; /* Ajusta el margen izquierdo según sea necesario */
  justify-content: space-between;
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

.cupon-code {
  display: flex;
  align-items: center; /* Alinea los elementos verticalmente */
}

.add-code {
  margin-left: 10px; /* Añade un espacio entre el input y el botón */
}
</style>
