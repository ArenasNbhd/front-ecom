<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantCar">
    <span style="text-transform: none; color: green">
      Fragant View
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaFragantCar () {
      this.$router.push('/velasSeis/velasSeisCar')
    }
  }
}
</script>
