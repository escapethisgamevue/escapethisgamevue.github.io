<script setup lang="ts">
import { ref } from "vue"

const animateRef = ref<any>()
function clickButton() {
    animateRef.value?.beginElement();
}
</script>

<template>
    <div class="h-fit w-fit" @click="clickButton()">
        <svg width="200mm" height="100mm" viewBox="0 0 200 100" version="1.1" class="svg1"
            xmlns="http://www.w3.org/2000/svg" xmlns:svg="http://www.w3.org/2000/svg">

            <rect style="fill:#04044c;fill-opacity:1;stroke:none;stroke-width:4.41684" id="rect1" width="200"
                height="100" x="-2.7755576e-17" y="0" ry="50" inkscape:label="background" sodipodi:insensitive="true" />
            <circle style="fill:#ffff00;fill-opacity:1;stroke:none;stroke-width:3.94714" class="path5" cx="56.027729"
                cy="49.629063" r="46.17075" />
            <circle style="fill:#04044c;fill-opacity:1;stroke:none;stroke-width:3.94714" class="path6" cx="71.915077"
                cy="39.37804" r="39.266808" />
        </svg>
    </div>
</template>

<style lang="scss">
.svg1:hover .path6 {
    // d: path("m 150.48196,5.7535847 a 45.186339,45.186339 0 0 0 -45.18622,45.1862263 45.186339,45.186339 0 0 0 45.18622,45.186227 45.186339,45.186339 0 0 0 41.19143,-26.65246 38.429597,38.429597 0 0 1 -25.64281,9.863221 38.429597,38.429597 0 0 1 -38.42941,-38.429407 38.429597,38.429597 0 0 1 22.98637,-35.1510408 45.186339,45.186339 0 0 0 -0.10558,-0.00277 z    ");
    r: 0;
    transform: translateY(-30px);
    transform: translateX(120px);
}

.svg1:hover .path5 {
    transform: translateX(90px);
    color: rgb(255, 166, 2);
}


svg polyline,
svg line,
svg circle {
    fill: none;
    stroke: #000;
    stroke-linecap: round;
    stroke-linejoin: round;
    transition: 1s;
}
</style>