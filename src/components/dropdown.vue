<script>
    import { ref } from 'vue';

    export default {
        'name': 'dropdown component',
        data() {
            return {
                'items': [
                    {
                        'display': 'github',
                        'path': 'https://github.com/'
                    },
                    {
                        'display': 'stack overflow',
                        'path': 'https://stackoverflow.com/'
                    },
                    {
                        'display': 'figma',
                        'path': 'https://www.figma.com/'
                    }
                ],
                'dropdown_active': false
            }
        },
        'methods': {
            dropdown(e) {
                if (e == 1) this.dropdown_active = true;
                else if (e == 2) this.dropdown_active = false;
            },
            choose_item(item) {
                console.log(item.path);
                window.open(item.path, '_blank');
            }
        }
    }
</script>

<template>
    <div @mouseover="dropdown(1)" @mouseleave="dropdown(2)" class="w-40 grid grid-cols-8 overflow-hidden bg-gray-600 justify-center items-center rounded-2xl border-4 border-gray-800 hover:border-gray-700" :class="{'bg-gray-500':this.dropdown_active}">
        <h1 class="col-span-6 text-center">Menu</h1>
        <i class="col-span-2 items-center justify-center fa-solid fa-chevron-down"></i>
        <div id="dropdown_container" class="flex flex-col w-full col-span-8" bg-green-500>
            <div @click="choose_item(item)" v-for="item in items" v-bind:class="[this.dropdown_active?'bg-gray-600 p-1 hover:bg-gray-500 flex justify-center items-center text-center':'hidden']">{{item.display}}</div>    
        </div>
    </div>
   
</template>

<style scoped>
    #dropdown_container:nth-child(2n) {
        @apply text-cyan-500
    }
</style>