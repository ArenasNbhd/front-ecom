<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCleanDetails">
    <span style="text-transform: none; color: green">
      Clean Car
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCleanDetails () {
      this.$router.push('/velasOcho/velasOchoCar/velasOchoDetails')
    }
  }
}
</script>
