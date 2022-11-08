<template>
  <div class="app">
    <header-app :links="links" :skils="skils"/>
  </div>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue'
export default {
  components: { HeaderApp },
  name: 'App',
  data ()
  {
    return {
      links: [
        { link: '/', nameLink: 'home' },
        { link: '/about', nameLink: 'about me' },
        { link: '/portfolio', nameLink: 'portfolio' },
        { link: '/contact', nameLink: 'contact' },
      ],
      skils: [
        { skil: 'Ux' },
        { skil: '</' },
        { skil: 'Ps' },
        { skil: 'UI' },
      ]
    }
  }  
  }
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600&display=swap');
*,*::after,*::before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  max-width: 1920px;
  margin: 0 auto;
  font-family: 'Montserrat', sans-serif;
}
.header {
  background: #2A2A2A;
  &__nav-wrapper {
    margin-left: 219px;
  }
  &__content {
    margin-top: 139px;
    display: flex;
  }
  &__top {
    padding-top: 26px;
    display: flex;
    align-items: center;
  }
  &__content-left {
    display: flex;
    flex-direction: column;
    max-width: 450px;
  }
  &__content-title {
    font-weight: 600;
    font-size: 48px;
    line-height: 54px;
    color: #E4E4E4;
    text-transform: uppercase;
    margin-bottom: 27px;
  }
  &__content-title-second {
    font-weight: 600;
    font-size: 72px;
    line-height: 82px;
    color: #E4E4E4;
    text-transform: uppercase;
    margin-bottom: 27px;
  }
  &__content-subtitle {
    font-weight: 300;
    font-size: 18px;
    line-height: 21px;
    color: #E4E4E4;
    margin-bottom: 27px;
  }
  &__content-right {
    position: relative;
    border: 67px solid #00C4F0;
    filter: drop-shadow(0px 0px 152px rgba(0, 196, 240, 0.42));
    border-radius: 50%;
    height: 575px;
    width: 575px;
    margin-left: 180px;
  }
  &__content-img {
    position: absolute;
    top: -126px;
    left: 0;
  }
  &__content-img-head {
    position: absolute;
    left: 0;
    top: -160px;
  }
  &__content-skil {
    list-style-type: none;
    background: linear-gradient(130.68deg, #414141 0%, #2D2D2D 100.52%);
    height: 90px;
    width: 90px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    font-weight: 700;
    font-size: 36px;
    line-height: 41px;
    color: #00C4F0;
    text-transform: uppercase;
  }
  &__content-skil:nth-child(1){
    left:-120px;
    top: 140px;
  }
  &__content-skil:nth-child(2){
    left: -60px;
    top: -20px;
  }
  &__content-skil:nth-child(3){
    left: -90px;
    top: 320px;
  }
  &__content-skil:nth-child(4){
    left: 350px;
    top: -50px;
  }
}
.container {
  padding: 0px 375px 0px 343px;
}
</style>
