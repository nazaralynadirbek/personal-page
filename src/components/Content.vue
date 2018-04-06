<template lang="pug">
    .content
        .top
            .about
                p
                  | Almaty-based web developer#[br]
                  | Currently building cool stuff using #[span(class='green') Vue]#[br]
                  | Student at the #[span(class='blue') Suleyman Demirel University]
        .bottom
            .group
                .title
                    h2 I know what you're here for
                .items
                    ul.list
                        li
                            a(href='https://github.com/naznadmn', target='_blank') Go and check some of my works
                        li
                            a(href='static/pdf/resume-06.04.18.pdf', target='_blank') Go and check my resume
                .additional
                    p I am always available for work
            .group.experience
                .title
                    h2 Experience
                .items
                    ul.list
                        li
                            h3 Web Development
                            p Node | Python, HTML, CSS & JS (Vue / Angular)
                        li
                            h3 Desktop Development
                            p Node, Electron & Vue
            .group.elsewhere
                .title
                    h2 Elsewhere
                .items
                    ul.list
                        li
                            a(href='https://vk.com/turnernne', target='_blank') vkontakte
                        li
                            a(href='https://www.npmjs.com/~naznadmn', target='_blank') npmjs
</template>

<script>
    export default {
        name: 'Content',

        props: {

        },

        data: function() {
            return {

            }
        }
    }
</script>

<style lang="scss">
    .content {
        color: #444;

        .top {
            margin-bottom: 40px;

            background: rgb(247,247,247);
            background: -moz-linear-gradient(top, rgba(247,247,247,1) 0%, rgba(226,226,226,1) 100%);
            background: -webkit-linear-gradient(top, rgba(247,247,247,1) 0%,rgba(226,226,226,1) 100%);
            background: linear-gradient(to bottom, rgba(247,247,247,1) 0%,rgba(226,226,226,1) 100%);
            filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f7f7f7', endColorstr='#e2e2e2',GradientType=0 );

            .about {
                width: 800px;
                margin: 0 auto;
                padding: 40px 0;

                p {
                    font-size: 30px;
                    font-weight: 300;
                    line-height: 48px;

                    span {
                        padding: 2px 6px;

                        &.green {
                            background-color: #c3fedd;
                        }
                        &.blue {
                            background-color: #c3e0fe;
                        }
                    }
                }
            }
        }
        .bottom {
            width: 800px;
            margin: 0 auto;

            .group {
                margin-bottom: 60px;

                .title {
                    margin-bottom: 20px;

                    h2 {
                        font-size: 14px;
                        font-weight: 700;
                    }
                }
                .items {
                    .list {
                        font-size: 0;

                        li {
                            margin-right: 60px;
                            padding-bottom: 10px;
                            display: inline-block;
                            border-bottom: 1px solid #d4d4d4;

                            a {
                                color: #444;
                                font-size: 18px;
                                padding-bottom: 10px;

                                &:hover {
                                    opacity: .7;
                                }
                            }

                            &:last-child {
                                margin-right: 0;
                            }
                        }
                    }
                }
                .additional {
                    margin-top: 20px;

                    p {
                        color: #9d9d9d;
                        font-size: 14px;
                    }
                }

                &.experience {
                    .items {
                        .list {
                            li {
                                padding: 0;
                                border: none;

                                h3 {
                                    font-size: 18px;
                                    font-weight: normal;
                                }
                                p {
                                    font-size: 14px;
                                    margin-top: 10px;
                                    font-weight: 300;
                                }
                            }
                        }
                    }
                }
                &.elsewhere {
                    .items {
                        .list {
                            li {
                                padding: 0;
                                border: none;

                                a {
                                    font-size: 14px;
                                }
                            }
                        }
                    }
                }

                &:last-child {
                    margin-bottom: 40px;
                }
            }
        }
    }
</style>
