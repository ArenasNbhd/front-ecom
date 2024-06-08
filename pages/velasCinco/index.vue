<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryCar">
    <span style="text-transform: none; color: green">
      Stary Golden
      View
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaStaryCar () {
      this.$router.push('/velasCinco/velasCincoCar')
    }
  }
}
</script>
