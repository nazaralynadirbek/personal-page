<template lang="pug">
    .container
        section-header()
        section-content()
        section-footer()
</template>

<script>
    import Header from './components/Header.vue';
    import Content from './components/Content.vue';
    import Footer from './components/Footer.vue';

    export default {
        name: 'App',

        components: {
            'section-header': Header,
            'section-content': Content,
            'section-footer': Footer
        },

        data: function() {
            return {

            }
        }
    }
</script>

<style lang="scss">
    @import "./style/desktop.css";

    .container {
        padding-top: 60px;
    }
</style>
