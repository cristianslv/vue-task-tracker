<template>
    <button 
        :style="`background: ${color}`" 
        @click="$emit('btn-click')"
        class="btn"
    >
    {{ text }}
    </button>
</template>

<script>
export default {
    name: "Button",
    props: {
        text: {
            type: String, 
            required: true,
            default: "Button"
        },
        color: {
            type: String,
            required: true,
            default: "lightgray"
        }
    }
}
</script>