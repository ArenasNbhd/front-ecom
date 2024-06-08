<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweerShipping">
    <span style="text-transform: none; color: green">
      Sweer Details
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSweerShipping () {
      this.$router.push('/velasDos/velasDosCar/velasDosDetails/velasDosShipping')
    }
  }
}
</script>
