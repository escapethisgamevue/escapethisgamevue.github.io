<script setup lang="ts">
import { ref } from "vue"

const animateRef = ref<any>()
function clickButton() {
    animateRef.value?.beginElement();
}
</script>

<template>
    <div class="h-fit w-fit" @click="clickButton()">
        <svg class="h-fit w-fit" width="102.635mm" height="102.635mm" viewBox="0 0 103 103" version="1.1" id="svg1"
            xmlns="http://www.w3.org/2000/svg" xmlns:svg="http://www.w3.org/2000/svg">

            <circle style="fill:#4d4d4d;stroke:#000000;stroke-width:3.01567" cx="51.50901" cy="51.479477" r="49.80949"
                id="Casing" />
            <circle style="fill:#9b0101;fill-opacity:1;stroke:#6d0101;stroke-width:2.63;stroke-opacity:1" cx="51.50901"
                cy="51.479477" r="35.757164" id="back-button" />
            <circle style="fill:#ff0000;stroke:#6d0101;stroke-width:2.63;stroke-opacity:1" cx="61.425705" cy="50.430336"
                r="35.757164" id="front-button">
                <animate ref="animateRef" attributeName="cx" begin="indefinite" values="61.425705;50.430336;61.425705"
                    dur="1s" repeatCount="1" />
            </circle>
        </svg>
    </div>
</template>