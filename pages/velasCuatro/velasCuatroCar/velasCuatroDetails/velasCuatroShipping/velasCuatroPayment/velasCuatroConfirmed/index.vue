<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaJuicyReturn">
    <span style="text-transform: none; color: green">
      Return to the initial page
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaJuicyReturn () {
      this.$router.push('/')
    }
  }
}
</script>
