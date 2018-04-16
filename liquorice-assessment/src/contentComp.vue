<template>
    <section>
        <div class="container">
            <content-desktop></content-desktop>
            <content-mobile></content-mobile>
        </div>
    </section>
</template>

<script>
    import contentDesktop from './contentDesktop.vue';
    import contentMobile from './contentMobile.vue';

    export default {
        components: {
            'content-desktop': contentDesktop,
            'content-mobile': contentMobile
        },
        data() {
            return {}
        }
    }
</script>
<style scoped lang = "scss" > 

</style>