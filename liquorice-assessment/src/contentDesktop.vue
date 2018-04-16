<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col col-tab-12">
                    <div class="breadcrumb">
                        <div class="breadcrumb__wrap">
                            <div class="breadcrumb-items">
                                <ul>
                                    <li v-for="items in listContent"> {{ items }}</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="content col-tab-6 col">
                    <div class="content__img">
                        <img src="./assets/img/historyimage.png" class="moirs-md img-responsive" alt="">
                    </div>
                </div>
                <div class="content col-tab-6 col">
                    <div class="content__text">
                        <h1 class="title">
                            <span>{{ pretitleContent }}</span>
                            {{ titleContent }}
                        </h1>
                        <p class="body" v-for="text in paragraphContent">{{ text }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        data() {
            return {
                pretitleContent: 'MOIR\'S',
                titleContent: 'History',
                listContent: ['Moir\'s', 'About Us', 'History'],
                paragraphContent: [
                    'MOIR\'S rich history of delicious desserts and bakes started back in the nineteenth century when Scotsman John Moir founded a business making fruit-flavoured jellies that proved immensely popular. ',
                    'The first MOIR\'S jelly to be produced in South Africa came from a factory in Woodstock just after the First World War. Instantly recognised for its fine quality, it inspired the introduction of other products. By 1950, MOIR\'S had expanded so much that the company had to move to Ndabeni.',
                    'Today, MOIR\'S is part of Pioneer Foods, the second biggest food group in the country, and is the leading brand when it comes to jellies, custards, and instant puddings - indeed a delectable tradition!'
                ]
            }
        }
    }
</script>
<style scoped lang = "scss" > 
    /* ==== COLOR ====== */
    $blue: #0e3267;
    $red: #d72d2d;

    .container {
        margin-bottom: 200px;
    }

    .breadcrumb {
        &__wrap {
            margin: 70px 0 90px;
            ul {
                list-style: none;
                text-align: center;

                li {
                    display: inline-block;
                    color: $blue;
                    text-transform: uppercase;
                    position: relative;
                        letter-spacing: 5px;
                    font-size: 20px;

                    &:before {
                        content: '';
                        width: 5px;
                        height: 5px;
                        position: absolute;
                        background-color: $blue;
                        border-radius: 50%;
                        top: 45%;
                        left: -15px;
                    }
                    
                    
                    &:not(:first-child) {
                        margin-left: 30px;
                    }

                    &:last-child {
                        color: $red;
                    }
                }
            }
        }
    }

    .content {
        &__text {
            padding-left: 50px;
            color: $blue;

            h1 {
                margin: 0;

                span {
                    font-size: 20px;
                    display: block;
                    font-weight: 300;
                }
            }

            p {
                font-weight: 300;
            }
        }
    }

    @media (min-width: 0) {
        .container {
            display: none;
        }
    }
    @media (min-width: 767px) {
        .container {
            display: block;
        }

        .content {
            &__text {
                h1 {
                    font-size: 70px;

                    span {
                        font-size: 20px;
                    }
                }

                p {
                    margin: 15px 0;
                    font-size: 15px;
                }
            }
        }
    }
    @media (min-width: 870px) {
        .content {
            &__text {
                h1 {
                    font-size: 80px;
                }

                p {
                    margin: 25px 0;
                    font-size: 16px;
                }
            }
        }
    }
    @media (min-width: 980px) {
        .content {
            &__text {
                p {
                    font-size: 20px;
                }
            }
        }
    }
    @media (min-width: 1024px) {
        .content {
            &__text {
                h1 {
                    font-size: 90px;
                }
                p {
                    margin: 30px 0;
                    font-size: 22px;
                }
            }
        }
    }
</style>