<template>
  <v-btn color="#E0E0E0" elevation="0" block @click="VelaFragantDetails">
    <span style="text-transform: none; color: green">
      Fragant Car
    </span>
  </v-btn>
</template>

<script>
export default {
  methods: {
    VelaFragantDetails () {
      this.$router.push('/velasSeis/velasSeisCar/velasSeisDetails')
    }
  }
}
</script>
