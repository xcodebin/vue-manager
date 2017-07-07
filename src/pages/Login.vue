<template>
  <div class="login">
    <VmLogin>
    </VmLogin>
    <tables ref="tablex"></tables>
  </div>
</template>
<script>
  import VmLogin from '@/components/vm-login'
//  import tables from '@/components/tables'
  export default {
    name: 'Login',
    components: {
      VmLogin
//      tables
    },
    mounted () {
      this.$refs.tablex.exportCsv()
    }
  }
</script>
