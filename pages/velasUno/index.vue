<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpicedCar">
    <span style="text-transform: none; color: green">
      Spiced View
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSpicedCar () {
      this.$router.push('/velasUno/velasUnoCar')
    }
  }
}
</script>
