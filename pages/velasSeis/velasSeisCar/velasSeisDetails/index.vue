<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantShipping">
    <span style="text-transform: none; color: green">
      Fragant Details
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaFragantShipping () {
      this.$router.push('/velasSeis/velasSeisCar/velasSeisDetails/velasSeisShipping')
    }
  }
}
</script>
