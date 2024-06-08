<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaStaryReturn">
    <span style="text-transform: none; color: green">
      Return to initial page
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaStaryReturn () {
      this.$router.push('/')
    }
  }
}
</script>
