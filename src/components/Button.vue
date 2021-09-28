<template>
    <button 
        :style="`background: ${color}`" 
        @click="onClick"
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
    },
    methods: {
        onClick() {
            console.log("click")
        }
    }
}
</script>