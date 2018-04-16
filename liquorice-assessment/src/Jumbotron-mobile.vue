<template>
    <div class="container-sm">
      <div class="jumbotron">
        <div class="jumbotron__content">
          <div class="content-item">  
            <span class="content-item__preheading">A little bit</span>
            <h1 class="content-item__title">About Moir’s</h1>

            <p class="content-item__content">For close to 100 years, MOIR'S has been a favourite in South African households, offering up scrumptious treats that the whole family can enjoy. Browse our product range by downloading the gull product listing below.</p>

            <button class="btn-default">Explore</button>
          </div>
        </div>
        <div class="jumbotron__image"> 
            <img src="./assets/img/mobile_bg.png" class="moirs-md" alt="">
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {}
        }
    }
</script>
<style scoped lang = "scss" >
  /* ==== COLOR ====== */ 
  $lightPink: #efbeb9;
  $white: #fff;

  * {
    box-sizing: border-box;
  }

  .jumbotron {
    position: relative;
    height: 100%;
    width: 100%;

    &__content {
      position: absolute;
      right: 50%;
      width: 400px;
      height: 400px;
      top: 50%;
      margin-top: -200px;
      border-radius: 50%;
      color: $white;
      line-height: 400px;
      color: $white;
      background: $lightPink;
      box-shadow: 5px 5px 47px 0px rgba(0, 0, 0, 0.1);
    }

    &__image {
      position: absolute;
      left: 30%;
      top: -10%;
      bottom: -10%;
      overflow: hidden;
      -webkit-transition: all .2s linear;
      -moz-transition: all .2s linear;
      -sm-transition: all .2s linear;
      transition: all .2s linear;

      img {
        height: 100%;
        width: 100%;
        object-fit: contain;
      }
    }
  }

  .content-item {
    line-height: 1;
    display: inline-block;
    padding: 50px;

    &__preheading {
      text-align: center;
      display: block;
      font-size: 30px;
      text-transform: uppercase;
    }

    &__title {
      font-size: 65px;
      line-height: 50px;
      margin: 0;
    }

    &__content {
      padding-left: 40px;
      font-size: 16px;
    }
  }

  .btn-default {
    background-color: transparent;
    border: 2px solid $white;
    color: $white;
    border-bottom-right-radius: 25px;
    border-top-left-radius: 25px;
    border-bottom-left-radius: 25px;
    border-top-right-radius: 25px;
    height: 45px;
    width: 220px;
    cursor: pointer;
    text-transform: uppercase;
    position: relative;
    top: 20px;
    left: -15px;
  }

@media (min-width: 0) and (max-width: 500px) {
  .container-sm {
    display: block;
    height: 750px;
  }
}

@media (min-width: 0) and (max-width: 346px) {
  .container-sm {
    display: block;
    height: 750px;
  }

  .jumbotron {
    &__content {
      right: 13%;
      width: 300px;
      height: 300px;
      top: 50%;
      margin-top: -200px;
    }

    &__image {
      top: -10%;
      bottom: -10%;
    }
  }

  .content-item {
    padding: 40px;

    &__preheading {
      font-size: 15px;
    }

    &__title {
      font-size: 40px;
      line-height: 40px;
    }

    &__content {
      padding-left: 10px;
      font-size: 10px;
      width: 150px;
    }
  }

  .btn-default {
    top: 150px;
    left: 15px;
  }
}

@media (min-width: 346px){
  .jumbotron {
    &__content {
      right: 15%;
      width: 300px;
      height: 300px;
      top: 50%;
      margin-top: -200px;
    }

    &__image {
      left: 32%;

      img{
        width: 120%;
      }
    }
  }

  .content-item {
    padding: 40px;

    &__preheading {
      font-size: 15px;
    }

    &__title {
      font-size: 40px;
      line-height: 40px;
    }

    &__content {
      padding-left: 10px;
      font-size: 10px;
      width: 150px;
    }
  }

  .btn-default {
    top: 150px;
    left: 15px;
  }
}

@media (min-width: 347px){
  .jumbotron {
    &__image {
      left: 34%;
      img{
        width: 110%;
      }
    }
  }
}

@media (min-width: 360px){
  .jumbotron {
    &__image {
      left: 36%;
    }
  }
}

@media (min-width: 365px){
  .content-item {
    &__content {
      width: 185px;
    }
  }
}

@media (min-width: 367px){
  .jumbotron {
    &__image {
      left: 48%;
    }
  }
}

@media (min-width: 460px){
  .jumbotron {
    &__image {
      left: 53%;
      img{
        width: 115%;
      }
    }
  }

  .content-item {
    &__content {
      font-size: 13px;
      width: 195px;
    }
  }
}

@media (min-width: 500px){
  .container-sm {
      display: none;
  }

  .jumbotron {
    &__content {
      right: 15%;
      width: 300px;
      height: 300px;
      top: 50%;
      margin-top: -200px;
    }

    &__image {
      left: 30%;
      top: -10%;
      bottom: -10%;
    }
  }

  .content-item {
    padding: 40px;

    &__preheading {
      font-size: 15px;
    }

    &__title {
      font-size: 40px;
      line-height: 40px;
    }

    &__content {
      padding-left: 10px;
      font-size: 10px;
    }
  }

  .btn-default {
    top: 150px;
    left: 15px;
  }
}
</style>