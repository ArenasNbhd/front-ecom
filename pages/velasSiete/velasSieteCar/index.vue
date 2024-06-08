<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemerDetails">
    <span style="text-transform: none; color: green">
      Sumemer car
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSumemerDetails () {
      this.$router.push('/velasSiete/velasSieteCar/velasSieteDetails')
    }
  }
}
</script>
