<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryConfirmed">
    <span style="text-transform: none; color: green">
      Stary Golden Payment
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaStaryConfirmed () {
      this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails/velasCincoShipping/velasCincoPayment/velasCincoConfirmed')
    }
  }
}
</script>
