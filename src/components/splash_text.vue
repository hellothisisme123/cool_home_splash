<script>
    import { ref } from 'vue';
    // import dropdown_component from '../components/dropdown.vue'

    
    export default {
        data() {
            return {
                'slider_width': 0
            }
        },
        'methods': {
            set_splash_width(e) {
                this.slider_width = (e.clientX / window.innerWidth) * 100;
                document.getElementById('slider').style.width = `${this.slider_width}%`
            }
        }
    }
</script>

<template>
    <div @mousemove="set_splash_width" class="w-full h-screen">
        <div id="slider" class="z-40 fixed left-0 top-0 bg-red-500 h-screen">
            <div class="z-10 text-[#242424] bg-transparent w-full h-screen flex overflow-hidden items-center">
                <h1 class="text-8xl text-center w-screen flex-none">Sexiest splash screen <br> on home <span class="text-blue-700 font-mono">effect</span> ever</h1>
            </div>
        </div>
        <div class="z-30 fixed top-0 left-0 bg-transparent w-full h-screen grid justify-items-center items-center grid-cols-1">
            <h1 class=" text-8xl text-center">Sexiest splash screen <br> on home <span class="text-purple-500 font-mono">effect</span> ever</h1>
        </div>
    </div>
</template>

<style scoped>
</style>
