<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCoolCar">
    <span style="text-transform: none; color: green">
      Cool view
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCoolCar () {
      this.$router.push('/velasTres/velasTresCar')
    }
  }
}
</script>
