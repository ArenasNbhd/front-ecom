<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyCar">
    <span style="text-transform: none; color: green">
      Juicy Lemon
      View
      9.99$
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaJuicyCar () {
      this.$router.push('/velasCuatro/velasCuatroCar')
    }
  }
}
</script>
