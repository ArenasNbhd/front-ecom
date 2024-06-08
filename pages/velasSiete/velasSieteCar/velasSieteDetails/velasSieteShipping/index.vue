<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemerPayment">
    <span style="text-transform: none; color: green">
      Sumemer shipping
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSumemerPayment () {
      this.$router.push('/velasSiete/velasSieteCar/velasSieteDetails/velasSieteShipping/velasSietePayment')
    }
  }
}
</script>
