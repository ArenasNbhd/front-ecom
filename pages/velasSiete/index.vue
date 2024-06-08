<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemerCar">
    <span style="text-transform: none; color: green">
      Sumemer view
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSumemerCar () {
      this.$router.push('/velasSiete/velasSieteCar')
    }
  }
}
</script>
