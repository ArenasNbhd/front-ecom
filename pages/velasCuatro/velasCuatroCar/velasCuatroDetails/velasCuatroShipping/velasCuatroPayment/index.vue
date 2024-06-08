<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyConfirmed">
    <span style="text-transform: none; color: green">
      Juicy Lemon
      Payment
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaJuicyConfirmed () {
      this.$router.push('/velasCuatro/velasCuatroCar/velasCuatroDetails/velasCuatroShipping/velasCuatroPayment/velasCuatroConfirmed')
    }
  }
}
</script>
