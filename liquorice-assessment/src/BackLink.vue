<template>
    <div class="backlink-wrap">
        <button class="backlink__item">{{ menuTitle}}</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                menuTitle: 'Back'
            }
        }
    }
</script>
<style scoped lang = "scss" > 
    /* ==== COLOR ====== */
    
    $white: #fff;

    .backlink-wrap {
        position: absolute;
        bottom: 5%;
        width: 95%;
        left: 5%;
        color: $white;
    
        &:before {
            content: url(./assets/img/arrow-left-icon.png);
            position: relative;
            top: 2px;
            margin-right: 10px;
        }
        
        button {
            background-color: transparent;
            color: $white;
            text-transform: uppercase;
            border: none;
            cursor: pointer;
            font-size: 20px;

            &:focus {
                outline: none;
            }
        }

    }

    @media (min-width: 0) {
        .backlink-wrap {
            display: none;
        }
    }

    @media (min-width: 768px) {
        .backlink-wrap {
            display: block;
        }
    }
</style>