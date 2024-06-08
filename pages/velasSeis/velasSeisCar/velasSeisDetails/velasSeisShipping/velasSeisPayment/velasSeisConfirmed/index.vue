<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantReturn">
    <span style="text-transform: none; color: green">
      Return
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaFragantReturn () {
      this.$router.push('/')
    }
  }
}
</script>
