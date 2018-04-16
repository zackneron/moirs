<template>
<section>
    <div class="container">
        <div class="row">
            <div class="content col-mob-12 col">
                <div class="content__text">
                    <h1 class="title">
                        <span>{{ pretitleContent }}</span>
                        {{ titleContent }}
                    </h1>

                    <p class="body">{{ paragraphContent1 }}</p>
                    <p class="body">{{ paragraphContent2 }}</p>
                    <p class="body"><img src="./assets/img/baker-img.png" class="img-responsive" alt=""></p>
                    <p class="body">{{ paragraphContent3 }}</p>
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
                paragraphContent1: 'MOIR\'S rich history of delicious desserts and bakes started back in the nineteenth century when Scotsman John Moir founded a business making fruit-flavoured jellies that proved immensely popular. ',
                img: '<img src="./assets/img/baker-img.png" class="img-responsive">',

                paragraphContent2: 'The first MOIR\'S jelly to be produced in South Africa came from a factory in Woodstock just after the First World War. Instantly recognised for its fine quality, it inspired the introduction of other products. By 1950, MOIR\'S had expanded so much that the company had to move to Ndabeni.',

                paragraphContent3: 'Today, MOIR\'S is part of Pioneer Foods, the second biggest food group in the country, and is the leading brand when it comes to jellies, custards, and instant puddings - indeed a delectable tradition!'
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

    .content {
        &__text {
            color: $blue;

            h1 {
                margin-top: 45px;
                font-size: 36px;

                span {
                    font-size: 11px;
                    display: block;
                    font-weight: 300;
                }
            }

            p {
                font-weight: 300;
                margin: 30px 0;
                font-size: 11px;
            }
        }
    }

    @media (min-width: 0) {
        .container {
            display: block;
        }
    }

    @media (min-width: 500px) {
        .content {
            &__text {
                h1 {
                    font-size: 50px;

                    span {
                        font-size: 16px;
                    }
                }

                p {
                    font-size: 16px;
                }
            }
        }
    }

    @media (min-width: 767px) {
        .container {
            display: none;
        }
    }
</style>