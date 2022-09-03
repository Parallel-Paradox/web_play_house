<template>
<button><span class="button_top">Button</span></button>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component';
export default class Button_1 extends Vue {}
</script>

<style scoped>
/* From uiverse.io by @Voxybuns */
button {
    /* Variables */
    --button_radius: 0.75em;
    --button_color: #e8e8e8;
    --button_outline_color: #000000;
    --button_thick: 0.3em;
    font-size: 17px;
    font-weight: bold;
    border: none;
    margin-top: var(--button_thick);
    border-radius: var(--button_radius);
    background: var(--button_outline_color);
}

.button_top {
    display: block;
    box-sizing: border-box;
    border: 2px solid var(--button_outline_color);
    border-radius: var(--button_radius);
    padding: 0.75em 1.5em;
    background: var(--button_color);
    color: var(--button_outline_color);
    transform: translateY(calc((-2 / 3) * var(--button_thick)));
    transition: transform 0.1s ease;
}

button:hover .button_top {
    /* Pull the button upwards when hovered */
    transform: translateY(calc((-1) * var(--button_thick)));
}

button:active .button_top {
    /* Push the button downwards when pressed */
    transform: translateY(0);
}
</style>
