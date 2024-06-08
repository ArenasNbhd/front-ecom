<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaSumemerReturn">
    <span style="text-transform: none; color: green">
      Return
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaSumemerReturn () {
      this.$router.push('/')
    }
  }
}
</script>
