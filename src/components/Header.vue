<template lang="pug">
    .header
        .left
            .logo
                h1 .nadirbek
        .right
            .menu
                ul.list
                    li
                        a(href='mailto:nazaraly.nadirbek@gmail.com') email
                    li
                        a(href='https://github.com/naznadmn', target='_blank') github
                    li
                        a(href='https://twitter.com/nazaraly_n', target='_blank') twitter
</template>

<script>
    export default {
        name: 'Header',

        props: {

        },

        data: function() {
            return {

            }
        }
    }
</script>

<style lang="scss">
    .header {
        color: #444;
        width: 800px;
        margin: 0 auto 40px;

        .left {
            float: left;

            .logo {
                h1 {
                    font-size: 16px;
                }
            }
        }
        .right {
            float: right;

            .menu {
                .list {
                    font-size: 0;

                    li {
                        font-size: 14px;
                        margin-right: 40px;
                        display: inline-block;

                        a {
                            color: #444;
                        }

                        &:last-child {
                            margin-right: 0;
                        }
                    }
                }
            }
        }

        &:after {
            content: '';
            clear: both;
            display: block;
        }
    }
</style>
