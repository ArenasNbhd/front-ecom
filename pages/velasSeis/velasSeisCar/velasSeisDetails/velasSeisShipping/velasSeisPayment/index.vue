<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantConfirmed">
    <span style="text-transform: none; color: green">
      Fragant Payment
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaFragantConfirmed () {
      this.$router.push('/velasSeis/velasSeisCar/velasSeisDetails/velasSeisShipping/velasSeisPayment/velasSeisConfirmed')
    }
  }
}
</script>
