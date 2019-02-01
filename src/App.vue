// template
<template>
    <div class="container">
        <h1>{{ message }}</h1>
        <p-button @click.native="decrement" :text="'-'"></p-button>
        <h3>{{ count }}</h3>
        <p-button @click.native="increment" :text="'+'"><p-button>
    </div>
</template>

// script
<script>
    import PButton from './Button'
    export default {
        name: 'App',
        components: {
            PButton
        },
        data() {
            return {
                message: 'Hello Parcel',
                count: 0
            }
        },
        methods: {
            increment () {
                this.count++
            },

            decrement () {
                this.count--
            }
        }
    }
</script>

// style
<style scroped lang="scss">
    $blue-color: blue;
    .container {
        width: 600px;
        margin: 50px auto;
        text-align: center;

        h1 {
            color: $blue-color;
        }
    }
</style>