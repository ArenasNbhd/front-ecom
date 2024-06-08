<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaCleanReturn">
    <span style="text-transform: none; color: green">
      Return
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaCleanReturn () {
      this.$router.push('/')
    }
  }
}
</script>
