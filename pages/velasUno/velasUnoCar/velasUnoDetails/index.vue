<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpicedShipping">
    <span style="text-transform: none; color: green">
      Spiced Details
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSpicedShipping () {
      this.$router.push('/velasUno/velasUnoCar/velasUnoDetails/velasUnoShipping')
    }
  }
}
</script>
