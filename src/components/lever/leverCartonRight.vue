<script setup lang="ts">
import { ref } from "vue"

const animateRef = ref<any>()
function clickButton() {
    console.log("clicked Lever")
    animateRef.value?.beginElement();
}
</script>

<template>
    <div class="h-fit w-fit" @click="clickButton()">
        <svg width="103mm" height="103mm" viewBox="0 0 103 103" version="1.1" id="svg1"
            xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd" xmlns="http://www.w3.org/2000/svg"
            xmlns:svg="http://www.w3.org/2000/svg">
            <defs id="defs1">
                <clipPath clipPathUnits="userSpaceOnUse" id="clipPath4">
                    <rect style="fill:#333333;stroke:none;stroke-width:2.63;stroke-opacity:1" id="rect5"
                        width="67.183197" height="221.79219" x="-18.312691" y="-11.123344" ry="33.591599" />
                </clipPath>
            </defs>
            <g id="layer1">
                <rect style="fill:#333333;stroke:none;stroke-width:2.30095;stroke-dasharray:none;stroke-opacity:1"
                    id="rect3" width="39.912464" height="99.609489" x="2.9409771" y="3.1261082" ry="21.715118" />
                <path id="rect1-6" style="fill:#808080;stroke:#000000;stroke-width:2.28244;stroke-dasharray:none"
                    d="m 20.72918,1.1938664 c -10.910507,0 -19.6939799,8.0390135 -19.6939799,18.0247746 v 64.807822 c 0,9.985765 8.7834729,18.024777 19.6939799,18.024777 h 5.010407 c 10.910502,0 19.69398,-8.039012 19.69398,-18.024777 V 19.218641 c 0,-9.9857611 -8.783478,-18.0247746 -19.69398,-18.0247746 z m 2.406258,8.4983575 c 7.685625,0 13.872941,6.6974021 13.872941,15.0166921 v 53.992491 c 0,8.31929 -6.187316,15.016695 -13.872941,15.016695 -7.685619,0 -13.872943,-6.697405 -13.872943,-15.016695 V 24.708916 c 0,-8.31929 6.187324,-15.0166921 13.872943,-15.0166921 z" />
                <g id="g5" transform="matrix(0.50506893,-0.19465339,0.21576205,0.46867424,-25.203093,8.153868)">
                    <rect style="fill:#4d4d4d;stroke:#000000;stroke-width:2.97746" id="rect2" width="152.44328"
                        height="27.798325" x="16.94434" y="75.499908" ry="12.335384"
                        transform="matrix(0.99999786,-0.00207065,0.00166046,0.99999862,0,0)" />
                    <circle
                        style="fill:#fe0000;fill-opacity:1;stroke:#9c0000;stroke-width:3.93;stroke-dasharray:none;stroke-opacity:1"
                        id="path5" cx="169.42461" cy="89.891647" r="30.846636" />
                    <animate ref="animateRef" attributeName="transform" begin="indefinite"
                        values="matrix(0.50506893,-0.19465339,0.21576205,0.46867424,-25.203093,8.153868);matrix(0.49904762,0.20960925,-0.16917134,0.48743191,9.473036,-1.1993696)"
                        dur="1s" repeatCount="1" />
                </g>
                <path id="rect1" style="fill:#808080;stroke:#000000;stroke-width:4.33;stroke-dasharray:none"
                    d="m 37.23752,1.1513509 c -19.801714,0 -35.7430376,15.9413241 -35.7430376,35.7430381 V 165.40799 c 0,19.80172 15.9413236,35.74304 35.7430376,35.74304 h 9.093502 c 19.801714,0 35.743038,-15.94132 35.743038,-35.74304 V 36.894389 c 0,-19.801714 -15.941324,-35.7430381 -35.743038,-35.7430381 z m 4.367176,16.8522011 c 13.948807,0 25.178308,13.280915 25.178308,29.778028 v 107.06685 c 0,16.49711 -11.229501,29.77803 -25.178308,29.77803 -13.948807,0 -25.178308,-13.28092 -25.178308,-29.77803 V 47.78158 c 0,-16.497113 11.229501,-29.778028 25.178308,-29.778028 z"
                    clip-path="url(#clipPath4)" transform="matrix(0.55098782,0,0,0.50428767,0.31065108,0.6286681)" />
            </g>
        </svg>



    </div>
</template>