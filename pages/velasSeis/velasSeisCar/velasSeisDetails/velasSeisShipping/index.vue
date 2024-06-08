<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantPayment">
    <span style="text-transform: none; color: green">
      Fragant Shipping
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaFragantPayment () {
      this.$router.push('/velasSeis/velasSeisCar/velasSeisDetails/velasSeisShipping/velasSeisPayment')
    }
  }
}
</script>
