<script setup>
import { computed } from 'vue'

const props = defineProps({
    alerta: {
        type: Object,
        required: true
    }
})

const isError = computed(() => {
    return 'Esta es la funcion'
})


</script>

<template>
    <div :class="isError" class="text-white text-center p-3 uppercase font-bold mb-3 rounded-md bg-red-500">
        {{ alerta.mensaje }}
    </div>
</template>