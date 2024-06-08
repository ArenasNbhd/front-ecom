<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyPayment">
    <span style="text-transform: none; color: green">
      Juicy Lemon
      Shipping
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaJuicyPayment () {
      this.$router.push('/velasCuatro/velasCuatroCar/velasCuatroDetails/velasCuatroShipping/velasCuatroPayment')
    }
  }
}
</script>
