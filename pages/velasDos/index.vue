<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSweerCar">
    <span style="text-transform: none; color: green">
      Sweer View
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSweerCar () {
      this.$router.push('/velasDos/velasDosCar')
    }
  }
}
</script>
