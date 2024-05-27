<template>
  <login-user />
</template>

<script>
import LoginUser from '@/components/users/PaginaInicio.vue' /* Esta es la primer página que despliega el ejecutar */

export default {
  name: 'IndexPage',
  components: {
    LoginUser
  },
  layout: 'login'
}
</script>
