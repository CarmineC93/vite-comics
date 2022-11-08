<script>
  import AppHeader from './components/AppHeader.vue';
  import AppContent from './components/AppContent.vue';
  import AppServicesList from './components/AppServicesList.vue';



  export default {
    components: {
      AppHeader,
      AppContent,
      AppServicesList
    }
  }
</script>

<template>  

  <AppHeader />
  <AppContent />
  <AppServicesList />

</template>

<style lang="scss">
@use "./styles/general.scss" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/partials/variables" as *;

</style>
