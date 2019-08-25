<template>
    <div class="container">
        <app-header></app-header>
        <hr>
        <div class="row">
            <app-server-list></app-server-list>
            <app-server-details></app-server-details>
        </div>
        <hr>
        <app-footer></app-footer>
    </div>
</template>

<script>
  import Header from './components/Shared/Header.vue';
  import Footer from './components/Shared/Footer.vue';
  import Servers from './components//Server/Servers.vue';
  import ServerDetails from './components/Server/ServerDetails.vue';
  
  export default {
    components: {
      'app-header': Header,
      'app-footer': Footer,
      'app-server-list': Servers,
      'app-server-details': ServerDetails,
    }
  }

</script>

<style>

</style>
