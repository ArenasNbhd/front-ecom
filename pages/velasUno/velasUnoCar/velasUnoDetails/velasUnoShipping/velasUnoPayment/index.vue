<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpicedConfirmed">
    <span style="text-transform: none; color: green">
      Spiced Payment
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSpicedConfirmed () {
      this.$router.push('/velasUno/velasUnoCar/velasUnoDetails/velasUnoShipping/velasUnoPayment/velasUnoConfirmed')
    }
  }
}
</script>
