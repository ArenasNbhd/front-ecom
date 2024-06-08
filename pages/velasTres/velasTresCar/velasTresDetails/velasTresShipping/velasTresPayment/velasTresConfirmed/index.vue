<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCoolReturn">
    <span style="text-transform: none; color: green">
      Return
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCoolReturn () {
      this.$router.push('/')
    }
  }
}
</script>
