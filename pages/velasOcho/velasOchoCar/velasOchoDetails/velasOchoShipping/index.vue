<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCleanPayment">
    <span style="text-transform: none; color: green">
      Clean Shipping
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCleanPayment () {
      this.$router.push('/velasOcho/velasOchoCar/velasOchoDetails/velasOchoShipping/velasOchoPayment')
    }
  }
}
</script>
