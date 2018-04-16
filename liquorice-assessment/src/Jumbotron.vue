<template>
<div class="container-md">
  <div class="jumbotron">
    <div class="jumbotron__content">
      <div class="content-item">  
      <span class="content-item__preheading">Just a bit</span>
      <h1 class="content-item__title">About Moir’s</h1>
      <p class="content-item__content">For close to 100 years, MOIR'S has been a favourite in South African households, offering up scrumptious treats that the whole family can enjoy. Browse our product range by downloading the gull product listing below.</p>

      <button class="btn-default">Moir’s History</button>
      </div>
    </div>
    <div class="jumbotron__image"> 
        <img src="./assets/img/web_bg.png" class="moirs-md">
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

@media (min-width: 0) {
  .container-md {
    display: none;
  }
}

@media (min-width: 500px){
  .container-md {
    display: block;
    height: 750px;
  }

  .jumbotron {
    &__content {
      right: 36%;
      width: 350px;
      height: 350px;
      top: 45%;
    }

    &__image {
      left: 46%;
      top: -30%;

      img {
        width: 133%;
      }
    }
  }

  .content-item {
    &__title {
      font-size: 50px;
    }

    &__content {
      padding-left: 40px;
      font-size: 12px;
    }
  }

  .btn-default {
      top: 140px;
      left: 50%;
  }
}

@media (min-width: 768px){
  .jumbotron {
    &__content {
      width: 400px;
      height: 400px;
    }

    &__image {
      left: 51%;
      top: -18%;
    }
  }

  .content-item {
    &__title {
      font-size: 55px;
    }

    &__content {
      font-size: 15px;
    }
  }

  .btn-default {
    top: 20px;
    left: -5%;
  }

}

@media (min-width: 971px){
  .jumbotron {
    &__content {
      right: 36%;
      top: 45%;
    }

    &__image {
      top: -10%;
      bottom: -10%;

      img {
        width: 108%;
      }
    }
  }

  .content-item {
    &__title {
      font-size: 65px;
    }

    &__content {
      font-size: 16px;
    }
  }

  .btn-default {
    left: -15px;
  }
}

@media (min-width: 1000px){
  .jumbotron {
    &__content {
      right: 40%;
    }

    &__image {
      left: 46%;
    }
  }
}

@media (min-width: 1024px){
  .jumbotron {
    &__content {
      right: 37%;
    }

    &__image {
      left: 50%;
    }
  } 
}

@media (min-width: 1100px){
  .jumbotron {
    &__content {
      right: 47%;
    }

    &__image {
      left: 41%;
      top: -5%;
      bottom: 0%;
    }
  }
}

@media (min-width: 1250px){
  .jumbotron {
    &__image {
      top: 0%;
    }
  }
}

@media (min-width: 1263px){
  .bg {
    height: auto;
  }

  .container-md {
    height: 950px;
  }

  .jumbotron {
    &__content {
      right: 40%;
      width: 700px;
      height: 700px;
      display: flex;
      top: 35%;
    }
    &__image {
      left: 35%;

      img {
        width: 124%;
      }
    }
  }

  .content-item {
    padding: 108px;
    align-self: center;

    &__preheading {
      font-size: 30px;
    }

    &__title {
      font-size: 140px;
      line-height: 105px;
    }

    &__content {
      padding-left: 80px;
      font-size: 16px;
      margin-top: 40px;
    }
  }

  .btn-default {
    font-size: 20px;
    top: 55px;
    left: -15%;
    width: 410px;
    height: 80px;
    border-bottom-right-radius: 50px;
    border-top-left-radius: 50px;
    border-bottom-left-radius: 50px;
    border-top-right-radius: 50px;
  }
}
</style>