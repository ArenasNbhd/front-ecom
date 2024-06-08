<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyDetails">
    <span style="text-transform: none; color: green">
      Juicy Lemon
      Car
      9.99$
    </span>
  </v-btn>
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
