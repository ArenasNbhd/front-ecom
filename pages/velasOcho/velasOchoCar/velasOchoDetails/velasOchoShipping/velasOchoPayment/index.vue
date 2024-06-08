<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCleanConfirmed">
    <span style="text-transform: none; color: green">
      Clean Payment
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCleanConfirmed () {
      this.$router.push('/velasOcho/velasOchoCar/velasOchoDetails/velasOchoShipping/velasOchoPayment/velasOchoConfirmed')
    }
  }
}
</script>
