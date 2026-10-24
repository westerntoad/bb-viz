<script setup>
import { ref, onMounted } from 'vue';

const selected = ref(Math.random() >= 0.5);
const darkSquare = ref(Math.random() >= 0.5);
</script>

<template>
    <div v-if='darkSquare'>
        <div class='darkSquare'></div>
    </div>
    <div v-if='!darkSquare'>
        <div class='lightSquare'></div>
    </div>
</template>