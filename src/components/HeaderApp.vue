<template>
  <header class="header container">
    <div class="header__inner">
      <div class="header__top">
        <div class="header__logo">
          <a href="" class="header__link-logo">
            <img src="@/assets/logo-header.png" alt="">
          </a>
        </div>
        <nav-menu class="header__nav-wrapper" :links="links" />
      </div>
      <div class="header__content">
        <div class="header__content-left">
          <h1 class="header__content-title">hello</h1>
          <h2 class="header__content-title-second">i’m sergey braychuk</h2>
          <h4 class="header__content-subtitle">I've been doing  front-end  development for a year now. Do you need a website ? Then contact me</h4>
          <button-page style="align-self:flex-start">Contact me</button-page>
        </div>
        <div class="header__content-right">
          <div class="header__content-img-wrapper">
            <img class="header__content-img" src="@/assets/bgimg.png" alt="" />
            <img src="@/assets/bghead.png" alt="" class="header__content-img-head">
          </div>
          <ul class="header__content-skils">
            <li class="header__content-skil" v-for="item in skils" :key="item.skil">{{item.skil}}</li>
          </ul>
        </div>
      </div>
    </div>
    
  </header>
</template>

<script>
import NavMenu from '@/components/NavMenu.vue'
import ButtonPage from '@/components/UI/ButtonPage.vue'
export default {
  name: 'header-app',
  components: {
    NavMenu,
    ButtonPage
  },
  props: {
    links: {
      type: Array,
      default: require
    },
    skils: {
      type: Array,
      defaault: require
    }
  }
  }
</script>

<style lang="scss" scoped>

</style>