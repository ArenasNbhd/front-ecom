<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCoolConfirmed">
    <span style="text-transform: none; color: green">
      Cool Payment
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCoolConfirmed () {
      this.$router.push('/velasTres/velasTresCar/velasTresDetails/velasTresShipping/velasTresPayment/velasTresConfirmed')
    }
  }
}
</script>
