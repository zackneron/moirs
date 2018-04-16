<template>
<div id ="v-wrapper">
    <app-header></app-header>	
    <app-content></app-content>
</div>
</template>

<script>
	import HeaderComp from './headerComp.vue';
	import ContentComp from './contentComp.vue';
	
    export default {
    	components: {
    		'app-header': HeaderComp,
    		'app-content': ContentComp
		},
        data() {
            return {
            
            }
        }
    }
</script>
<style scoped lang = "scss" > 

</style>