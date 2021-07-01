<template>
    <img class="top-theme" alt="Vue logo" src="./assets/home/1.png">
    <swiper @subevent="onTestClick" :url="m3" :num="a" ></swiper>
</template>


<script>
    import Swiper from "@/components/Swiper";
    import m3 from '@/assets/home/2.png';
    import {ref} from  'vue'

    let a = ref(1)
    export default {
        name: 'App',
        components: {
            Swiper,
        },
        setup(){
            function onTestClick(event) {
                console.log(event)
            }

            return{
                m3,
                a,
                onTestClick
            }
        }
    }
</script>

<style>


    .top-theme {
        width: 100%;

    }
</style>
