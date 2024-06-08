<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemerShipping">
    <span style="text-transform: none; color: green">
      Sumemer details
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSumemerShipping () {
      this.$router.push('/velasSiete/velasSieteCar/velasSieteDetails/velasSieteShipping')
    }
  }
}
</script>
