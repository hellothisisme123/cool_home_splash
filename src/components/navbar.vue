<script>
    import { ref } from 'vue';
    // import dropdown_component from '../components/dropdown.vue'
    import dropdown from './dropdown.vue'
    import pillBtn from './pill_btn.vue'

    export default {
        components: {
            dropdown,
            pillBtn
        }
    }
</script>

<template>
    <div class="mt-4 grid grid-cols-2 justify-items-center bg-transparent w-full fixed text-gray-100">
        <div class="flex gap-3">
            <h1 class="text-xl drop-shadow-2xl">Website</h1>
            <dropdown></dropdown>
        </div>
        <pillBtn></pillBtn>
    </div>
</template>

<style scoped>

</style>
