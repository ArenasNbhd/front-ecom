<template>
  <v-card
    color="#84FFFF"
    elevation="0"
    width="500"
  >
    <v-card-title>
      Inicio de Sesión
    </v-card-title>
    <v-card-text>
      <v-form
        ref="form"
        v-model="validForm"
      >
        Email:
        <v-text-field
          v-model="email"
          placeholder="Escribe tu correo"
          type="email"
          :rules="correo"
        />
        Password:
        <v-text-field
          v-model="passwordUser"
          placeholder="Escribe tu password"
          type="password"
          :rules="password"
        />
      </v-form>
    </v-card-text>
    <v-card-actions>
      <v-row>
        <v-col cols="6">
          <v-btn block color="#212121" elevation="0" @click="loginUser">
            <span style="text-transform: none; color: white">
              Login
            </span>
          </v-btn>
        </v-col>
        <v-col cols="6">
          <v-btn block color="#BDBDBD" elevation="0" @click="showNuevo = true">
            <span style="text-transform: none; color: white">
              Signup
            </span>
          </v-btn>
        </v-col>
      </v-row>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {

}
</script>
