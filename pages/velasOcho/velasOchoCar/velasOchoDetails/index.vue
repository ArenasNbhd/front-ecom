<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCleanShipping">
    <span style="text-transform: none; color: green">
      Clean Details
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCleanShipping () {
      this.$router.push('/velasOcho/velasOchoCar/velasOchoDetails/velasOchoShipping')
    }
  }
}
</script>
