<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweerConfirmed">
    <span style="text-transform: none; color: green">
      Sweer Payment
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSweerConfirmed () {
      this.$router.push('/velasDos/velasDosCar/velasDosDetails/velasDosShipping/velasDosPayment/velasDosConfirmed')
    }
  }
}
</script>
