<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCoolPayment">
    <span style="text-transform: none; color: green">
      Cool Shipping
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCoolPayment () {
      this.$router.push('/velasTres/velasTresCar/velasTresDetails/velasTresShipping/velasTresPayment')
    }
  }
}
</script>
