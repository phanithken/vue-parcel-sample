// template
<template>
    <button>{{ text }}</button>
</template>

// script
<script>
    export default {
        name: 'p-button',
        props: {
            text: { required: true }
        },
        data() {
            return {
                message: ""
            }
        }
    }
</script>

// style
<style scoped lang="scss">
    button {
        height: 50px;
        width: 50px;
        color: white;
        border: none;
        background: black;
        border-radius: 5px;
    }
</style>
