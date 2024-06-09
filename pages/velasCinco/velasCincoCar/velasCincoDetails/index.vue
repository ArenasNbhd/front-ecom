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
        <p style="color: black">
          >  Details
        </p>
        <p style="color: gray;">
          > Shipping
        </p>
        <p style="color: gray;">
          >  Payment
        </p>
      </div>

      <div class="contact">
        <h2>Contact</h2>
        <p>
          Do you hace an account?
          <v-btn color="white" @click="showLogin = true">
            <span style="text-transform: none; color: green">
              Login
            </span>
          </v-btn>
        </p>
      </div>

      <v-dialog v-model="showLogin" max-width="500" persistent>
        <v-card>
          <v-card-tittle class="headline">
            Welcome, dear new user.
          </v-card-tittle>
          <v-card-text>
            Follow the instructions and answer the fields.
            <v-form
              ref="form"
              v-model="validForm"
            >
              <v-text-field
                v-model="email"
                label="Email"
                placeholder="Write your Email"
                color="#558B2F"
                type="email"
                :rules="correo"
              />
              <v-text-field
                v-model="passwordUser"
                label="Password"
                type="password"
                placeholder="Write your Password"
                color="#558B2F"
                :rules="password"
              />
              <v-text-field
                v-model="numeroUser"
                label="Número Telefónico"
                type="numero"
                placeholder="Write your Phone Number"
                color="#558B2F"
                :rules="number"
              />
            </v-form>
          </v-card-text>
          <v-card-actions>
            <v-row>
              <v-col cols="6">
                <v-btn color="red darken-1" elevation="0" block @click="showLogin = false">
                  <span style="text-transform: none; color: white">
                    Cancelar
                  </span>
                </v-btn>
              </v-col>
              <v-col cols="6">
                <v-btn color="green darken-1" elevation="0" block @click="LoginUser">
                  <span style="text-transform: none; color: white">
                    Iniciar Sesión
                  </span>
                </v-btn>
              </v-col>
            </v-row>
          </v-card-actions>
        </v-card>
      </v-dialog>

      <v-btn color="white" @click="newSignup">
        <span style="text-transform: none; color: green">
          Check Signup
        </span>
      </v-btn>

      <v-form
        ref="formNew"
        v-model="validFormNew"
      >
        <div class="cuadro">
          <v-text-field
            v-model="emailNuevo"
            placeholder="Email or mobile phone number"
            label="Email"
            color="#558B2F"
            type="email"
            :rules="correo"
          />
          <v-text-field
            v-model="passwordUserNueva"
            placeholder="Write your Password"
            label="Password"
            color="#558B2F"
            type="password"
            :rules="password"
          />
        </div>

        <div class="boton">
          <input type="checkbox"><p>Add me to Candleaf newsletter for a 10% discount</p>
        </div>

        <div>
          <h2>
            Shipping Address
          </h2>
        </div>

        <div class="cuadro2">
          <v-text-field
            v-model="name"
            placeholder="Name"
            label="Name"
            color="#558B2F"
            type="name"
          />
          <v-text-field
            v-model="secname"
            placeholder="Second Name"
            label="Second Name"
            color="#558B2F"
            type="name"
          />
        </div>

        <div class="cuadro">
          <v-text-field
            v-model="adress"
            placeholder="Adress and Number"
            label="Adress and Number"
            color="#558B2F"
            type="text"
          />
          <v-text-field
            v-model="numeroUserNuevo"
            placeholder="Phone Number"
            label="Phone Number"
            color="#558B2F"
            type="number"
            :rules="number"
          />
        </div>

        <div class="cuadro">
          <input type="text" placeholder="Shipping note (optional)">
        </div>

        <div class="cuadro2">
          <v-text-field
            v-model="city"
            placeholder="City"
            label="City"
            color="#558B2F"
            type="text"
          />
          <v-text-field
            v-model="cp"
            v-form
            placeholder="Postal Code"
            label="Postal Code"
            color="#558B2F"
            type="number"
            :rules="postal"
          >
            <select>
              <option value="" disabled selected hidden>
                Selecciona Providencia &#9660;
              </option>
              <option value="">
                Providencia 1
              </option>
              <option value="">
                Providencia 2
              </option>
              <option value="">
                Providencia 3
              </option>
              <option value="">
                Providencia 4
              </option>
            </select>
          <!-- Agrega más opciones según sea necesario -->
          </v-text-field>
        </div>

        <div class="cuadro">
          <select>
            <option value="" disabled selected hidden>
              Country/Region &#9660;
            </option>
            <option value="Italy">
              italy
            </option>
            <option value="Mexico">
              Mexico
            </option>
            <option value="Mexico">
              USA
            </option>
            <option value="Mexico">
              Valle de Santiago
            </option>
          <!-- Agrega más opciones según sea necesario -->
          </select>
        </div>
      </v-form>

      <div class="boton">
        <input type="checkbox"><p>Save this informations for future fast checkout</p>
      </div>

      <div class="finalcontainer">
        <v-btn color="white" @click="backCart">
          <span style="text-transform: none; color: green">
            Back to cart
          </span>
        </v-btn>
      </div>
      <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryShipping">
        <span style="text-transform: none; color: green">
          Go to shipping
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
  data () {
    return {
      showLogin: false,
      validFormNew: false,
      validForm: false,
      emailNuevo: null,
      passwordUserNueva: null,
      email: null,
      passwordUser: null,
      numeroUser: null,
      numeroUserNuevo: null,
      name: null,
      secname: null,
      adress: null,
      city: null,
      cp: null,
      required: [
        v => !!v || 'Required Field'
      ],
      password: [
        v => (v && v.length > 6) || 'Password must be more than 6 chars'
      ],
      correo: [
        v => /.+@.+\..+/.test(v) || 'E-mail must be valid'
      ],
      number: [
        v => (v && v.length > 9) || 'Password must be more than 6 chars'
      ],
      postal: [
        v => (v && v.length < 7) || 'Password must be more than 6 chars'
      ]
    }
  },
  methods: {
    VelaStaryShipping () {
      this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails/velasCincoShipping')
    },
    backCart () {
      this.$router.push('/velasCinco/velasCincoCar')
    },
    LoginUser () {
      this.validForm = this.$refs.form.validate()
      if (this.validForm) {
        // Si se puede loggear, enviamos una alerta
        const sendData = {
          email: this.email,
          password: this.passwordUser,
          numero: this.numeroUser
        }
        const url = '/login'
        this.$axios.post(url, sendData)
          .then((res) => {
            console.log('@@ res => ', res)
            if (res.data.token) {
              localStorage.setItem('token', res.data.token)
              this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails/velasCincoShipping')
              // Redirigir a la siguiente página
            }
          })
          .catch((err) => {
            console.log('@@ err => ', err)
          })
      } else {
        alert('Algo salió mal:(')
      }
    },
    newSignup () {
      this.validFormNew = this.$refs.formNew.validate()
      if (this.validFormNew) {
        const sendData = {
          id: Date.now().toLocaleString(),
          email: this.emailNuevo,
          password: this.passwordUserNueva,
          numero: this.numeroUserNuevo,
          name: this.name,
          secname: this.secname,
          adress: this.adress,
          city: this.city,
          cp: this.cp
        }
        console.log('@@@ data => ', sendData)
        const url = '/signup'
        this.$axios.post(url, sendData)
          .then((res) => {
            console.log('@@ res => ', res)
          })
          .catch((err) => {
            console.log('@@ err => ', err)
          })
      } else {
        alert('Faltan Datos')
      }
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

.login {
  color: green;
  text-decoration: underline;
  text-align: center;
}

.contact {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.cuadro {
  border: 1px solid green; /* Contorno verde */
  display: flex;
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
  cursor: pointer;
  flex-grow: 1;
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
