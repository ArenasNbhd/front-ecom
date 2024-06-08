<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpicedPayment">
    <span style="text-transform: none; color: green">
      Spiced Shipping
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSpicedPayment () {
      this.$router.push('/velasUno/velasUnoCar/velasUnoDetails/velasUnoShipping/velasUnoPayment')
    }
  }
}
</script>
