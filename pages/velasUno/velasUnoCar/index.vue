<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpicedDetails">
    <span style="text-transform: none; color: green">
      Spiced Car
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSpicedDetails () {
      this.$router.push('/velasUno/velasUnoCar/velasUnoDetails')
    }
  }
}
</script>
