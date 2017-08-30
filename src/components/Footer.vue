<template lang="pug">
    .footer
        .copyright
            p © Nazaraly Nadirbek 2017
</template>

<script>
    export default {
        name: 'Footer',

        props: {

        },

        data: function() {
            return {

            }
        }
    }
</script>

<style lang="scss">
    .footer {
        width: 800px;
        margin: 0 auto;
        padding-bottom: 40px;

        .copyright {
            color: #9d9d9d;
            font-size: 14px;
        }
    }
</style>
