<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSpicedReturn">
    <span style="text-transform: none; color: green">
      Return
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSpicedReturn () {
      this.$router.push('/')
    }
  }
}
</script>
