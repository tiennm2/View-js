<template>
  <div class="wrapper">
    <Header/>
    <Sidebar/>
    <div class="content-wrapper">
      <nuxt/>
    </div>
    <Footer/>
  </div>
</template>

<script>
  import Header from '~/components/layout/Header'
  import Footer from '~/components/layout/Footer'
  import Sidebar from '~/components/layout/Sidebar'

  export default {
    head() {
      return {
        script: [
          //jquery
          {src: '/admin/components/plugins/jquery/jquery.min.js'},
          //jquery UI
          {src: '/admin/components/plugins/jquery-ui/jquery-ui.min.js'},
          //bootstrap 4
          {src: '/admin/components/plugins/bootstrap/js/bootstrap.bundle.min.js'},
          //admin LTE
          {src: '/admin/components/dist/js/adminlte.js'},
          //  datatable
          {src: '/admin/components/plugins/datatables/jquery.dataTables.min.js'},
          //  main.js
          {src: '/admin/components/dist/js/main.js'},

        ],
        link: [
          {rel: 'stylesheet', href: '/admin/components/plugins/fontawesome-free/css/all.min.css'},
          {rel: 'stylesheet', href: '/admin/components/dist/css/adminlte.min.css'},
          {rel: 'stylesheet', href: '/admin/components/dist/css/main.css'},
          {rel: 'stylesheet', href: '/admin/components/plugins/overlayScrollbars/css/OverlayScrollbars.min.css'},
          {rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700'},

        ]
      }
    },
    name: "admin",
    components: {
      Sidebar,
      Header,
      Footer,
    },
  }
</script>

<style scoped lang="scss">
  @import "~/assets/scss/main.scss";
</style>
