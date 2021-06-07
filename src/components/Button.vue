<template>
    <button @click="onClick()" :style="{background: color}" class="btn">
        {{ title }}
    </button>
</template>

<script>
export default {
    name: "Button",
    props: {
        title: {
            type: String,
            default: "Default Title"
        },
        color: {
            type: String,
            default: "#feaf12"
        }
    },
    methods: {
        onClick() {
            console.log('clicked')
        }
    }
}
</script>