<template>
    <Button_1/>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Button_1 from './components/button/Button_1.vue';

@Options({
    components: {
        Button_1,
    },
})
export default class App extends Vue {}
</script>
