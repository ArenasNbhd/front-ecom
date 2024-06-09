<template>
  <!--<div class="FondoPantalla"></div>-->
  <!--Es correcto-->
  <div>
    <!-- Barra de Navegación -->
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

    <!-- Ventanas modales -->
    <v-dialog v-model="showSignup" max-width="500" persistent>
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
              <v-btn color="blue darken-1" elevation="0" block @click="showSignup = false">
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
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpiced">
          <span style="text-transform: none; color: green">
            Spiced Mint
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P2.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweer">
          <span style="text-transform: none; color: green">
            Sweer Strawberry
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P3.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaCool">
          <span style="text-transform: none; color: green">
            Cool Blueberries
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P4.png" alt="Imagen 1">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicy">
          <span style="text-transform: none; color: green">
            Juicy Lemon
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P5.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaStary">
          <span style="text-transform: none; color: green">
            Stary Golden
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P6.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragant">
          <span style="text-transform: none; color: green">
            Fragant Cinnamon
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P7.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemer">
          <span style="text-transform: none; color: green">
            Sumemer Cherries
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P8.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaClean">
          <span style="text-transform: none; color: green">
            Clean Lavander
            9.99$
          </span>
        </v-btn>
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
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpiced">
          <span style="text-transform: none; color: green">
            Spiced Mint
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P2.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweer">
          <span style="text-transform: none; color: green">
            Sweer Strawberry
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P3.png" alt="Imagen 2">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaCool">
          <span style="text-transform: none; color: green">
            Cool Blueberries
            9.99$
          </span>
        </v-btn>
      </div>
      <div class="grid-item">
        <img src="@/img/P4.png" alt="Imagen 1">
        <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicy">
          <span style="text-transform: none; color: green">
            Juicy Lemon
            9.99$
          </span>
        </v-btn>
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
  data () {
    return {
      showSignup: false,
      validForm: false,
      email: null,
      passwordUser: null,
      numeroUser: null,
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
      ]
    }
  },
  methods: {
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

              // this.$router.push('/components/users/PaginaInicio.vue')
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
    SignupUser () {
    },
    VelaSpiced () {
      this.$router.push('/velasUno')
    },
    VelaSweer () {
      this.$router.push('/velasDos')
    },
    VelaCool () {
      this.$router.push('/velasTres')
    },
    VelaJuicy () {
      this.$router.push('/velasCuatro')
    },
    VelaStary () {
      this.$router.push('/velasCinco')
    },
    VelaFragant () {
      this.$router.push('/velasSeis')
    },
    VelaSumemer () {
      this.$router.push('/velasSiete')
    },
    VelaClean () {
      this.$router.push('/velasOcho')
    }
  }
}
</script>

<style scoped>

.FondoPantalla {
  background-image: url('@/img/FondoP.jpg'); /* Ruta a tu imagen */
  background-size: cover; /* Ajusta la imagen para que cubra todo el fondo */
  background-repeat: no-repeat; /* Evita que la imagen se repita */
  background-position: center; /* Centra la imagen */
  min-height: 100vh; /* Asegura que el contenedor cubra al menos la altura de la ventana */
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
