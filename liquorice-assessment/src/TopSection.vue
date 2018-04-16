<template>
    <div class="top-nav">
        <div class="logo-wrap">
            <div class="logo-item">
                <a href="#">
                    <img src="src/assets/img/moirslogo.png" alt="MOIR'S logo" />
                </a>
            </div>
        </div>
        <div class="menu-wrap">
            <div class="menu-item">
                <div class="search-block">
                    <a href="#">search</a>
                </div>
                <a href="#" class="menu-item__target">{{ menuTitle}}</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                menuTitle: 'Menu'
            }
        }
    }
</script>

<style scoped lang = "scss" > 
    .top-nav {
        display: flex;
        align-items: flex-end;
        position: absolute;
        width: 100%;
        z-index: 10;

        .logo-wrap {
            position: relative;
            top: 0;
            left: 5%;
            width: 50%;
    
        }

        .logo-item {
            

            img {
                width: 100%;
                -webkit-transition: max-width .5s linear;
                -moz-transition: max-width .5s linear;
                -sm-transition: max-width .5s linear;
                transition: max-width .5s linear;
            }
        }

        .menu-wrap {
            position: relative;
            right: 5%;
            width: 50%;
            text-align: right;

            .menu-item {
                &__target {
                    color: white;
                    text-decoration: none;
                    text-transform: uppercase;
                    font-size: 21px;
                }

                .search-block {
                    position: relative;
                    display: inline-block;
                        
                    &:before {
                        content: url(./assets/img/search-icon.png);
                        position: absolute;
                        top: -6px;
                        right: 10px;
                        opacity: 1;
                    }

                    a {
                        
                        width: 30px;
                        opacity: 0;
                    }
                }
            }
        }
    }

@media (min-width: 767px){
    .top-nav {
        .logo-item {
            img {
                max-width: 150px;
            }
        }
    }
}

@media (min-width: 0) and (max-width: 767px) {
    .top-nav {
        .logo-item {
            img {
                max-width: 70px;
            }
        }
    }
}
</style>