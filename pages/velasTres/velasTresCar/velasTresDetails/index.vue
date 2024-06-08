<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCoolShipping">
    <span style="text-transform: none; color: green">
      Cool Details
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCoolShipping () {
      this.$router.push('/velasTres/velasTresCar/velasTresDetails/velasTresShipping')
    }
  }
}
</script>
