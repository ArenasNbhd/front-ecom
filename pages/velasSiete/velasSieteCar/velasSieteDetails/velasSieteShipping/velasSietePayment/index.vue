<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemerConfirmed">
    <span style="text-transform: none; color: green">
      Sumemer payment
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSumemerConfirmed () {
      this.$router.push('/velasSiete/velasSieteCar/velasSieteDetails/velasSieteShipping/velasSietePayment/velasSieteConfirmed')
    }
  }
}
</script>
