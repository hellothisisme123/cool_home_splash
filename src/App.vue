<script>
  // import HelloWorld from './components/HelloWorld.vue'
  // import header from './components/header.vue'
  // import dropdown_component from './components/dropdown.vue'
  // import dropdown from './components/dropdown.vue'
  import navbar from './components/navbar.vue';
  import dropdown from './components/dropdown.vue';
  import splash_text from './components/splash_text.vue';

  export default {
    components: {
      navbar,
      dropdown,
      splash_text
    }
  }

</script>

<template>
  <div>
    <navbar class="z-50"></navbar>
    <splash_text></splash_text>
  </div>
  <!-- <HelloWorld msg="Vite + Vue" /> -->
</template>

<style scoped>

</style>