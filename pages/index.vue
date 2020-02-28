<template>
  <div>
    <user-list/>
  </div>
</template>

<script>
  import AppLogo from '~/components/AppLogo.vue'
  import FrontendBase from '~/components/layout/FrontendBase'
  import UserList from '~/components/user/List'

  export default {
    head(){
      return{
        title: 'User Management',
      }
    },
    extends: FrontendBase,
    layout: 'admin',
    components: {
      AppLogo,
      UserList
    }
  }
</script>

<style>
</style>

