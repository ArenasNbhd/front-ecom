<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryPayment">
    <span style="text-transform: none; color: green">
      Stary Golden Shipping
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaStaryPayment () {
      this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails/velasCincoShipping/velasCincoPayment')
    }
  }
}
</script>
