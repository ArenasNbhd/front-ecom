<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweerPayment">
    <span style="text-transform: none; color: green">
      Sweer Shipping
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSweerPayment () {
      this.$router.push('/velasDos/velasDosCar/velasDosDetails/velasDosShipping/velasDosPayment')
    }
  }
}
</script>
