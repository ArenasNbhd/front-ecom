<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweerDetails">
    <span style="text-transform: none; color: green">
      Sweer Car
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSweerDetails () {
      this.$router.push('/velasDos/velasDosCar/velasDosDetails')
    }
  }
}
</script>
