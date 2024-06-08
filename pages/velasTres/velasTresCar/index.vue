<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCoolDetails">
    <span style="text-transform: none; color: green">
      Cool Car
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCoolDetails () {
      this.$router.push('/velasTres/velasTresCar/velasTresDetails')
    }
  }
}
</script>
