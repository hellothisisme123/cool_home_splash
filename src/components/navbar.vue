<script>
    import { ref } from 'vue';
    // import dropdown_component from '../components/dropdown.vue'
    import dropdown from './dropdown.vue'

    export default {
        components: {
            dropdown
        }
    }
</script>

<template>
    <div class="flex bg-transparent w-full fixed text-gray-100">
        <h1>Website</h1>
        <dropdown></dropdown>
    </div>
</template>

<style scoped>

</style>
