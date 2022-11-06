<script>
  // import HelloWorld from './components/HelloWorld.vue'
  // import header from './components/header.vue'
  // import dropdown_component from './components/dropdown.vue'
  // import dropdown from './components/dropdown.vue'
  import navbar from './components/navbar.vue'
  import dropdown from './components/dropdown.vue';

  export default {
    components: {
      navbar,
      dropdown
    }
  }

</script>

<template>
  <div>
    <navbar></navbar>
  </div>
  <!-- <HelloWorld msg="Vite + Vue" /> -->
</template>

<style scoped>

</style>