<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCleanCar">
    <span style="text-transform: none; color: green">
      Clean View
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCleanCar () {
      this.$router.push('/velasOcho/velasOchoCar')
    }
  }
}
</script>
