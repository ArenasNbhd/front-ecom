<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyShipping">
    <span style="text-transform: none; color: green">
      Juicy Lemon
      Details
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaJuicyShipping () {
      this.$router.push('/velasCuatro/velasCuatroCar/velasCuatroDetails/velasCuatroShipping')
    }
  }
}
</script>
