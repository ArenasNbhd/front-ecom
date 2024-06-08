<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryDetails">
    <span style="text-transform: none; color: green">
      Stary Golden
      Car
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaStaryDetails () {
      this.$router.push('/velasCinco/velasCincoCar/velasCincoDetails')
    }
  }
}
</script>
