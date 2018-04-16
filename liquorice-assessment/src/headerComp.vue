<template>
    <header class="bg">
        <header-top></header-top>
        <header-jumbotron></header-jumbotron>
        <header-jumbotron-mobile></header-jumbotron-mobile>
        <header-backlink></header-backlink>
    </header>
</template>

<script>
    import TopSection from './TopSection.vue';
    import Jumbotron from './Jumbotron.vue';
    import JumbotronMobile from './Jumbotron-mobile.vue';
    import BackLink from './BackLink.vue';
    export default {
        components: {
            'header-top': TopSection,
            'header-jumbotron': Jumbotron,
            'header-jumbotron-mobile': JumbotronMobile,
            'header-backlink': BackLink
        },
        data() {
            return {
            
            }
        }
    }
</script>
<style scoped lang = "scss" > 
    /* ==== COLOR ====== */
    $primary: #ed9a94;

    .bg {
        background: $primary url('./assets/img/header-bg.png') 50% 50% / cover no-repeat;
    }
    
    @media (min-width: 767px){
        .bg {
            height: 650px;
            position: relative;
        }
    }
    @media (min-width: 1250px){
        .bg {
            height: auto;
        }
    }
</style>