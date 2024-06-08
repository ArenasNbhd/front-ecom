<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryShipping">
    <span style="text-transform: none; color: green">
      Stary Golden Details
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaStaryShipping () {
      this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails/velasCincoShipping')
    }
  }
}
</script>
