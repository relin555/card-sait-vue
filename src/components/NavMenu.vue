<template>
  <div class="nav">
        <nav class="nav__menu">
          <ul class="nav__items">
            <li class="nav__item" v-for="item in links" :key="item.link">
              <a :href="item.link" class="nav__link">{{ item.nameLink }}</a>
            </li>
          </ul>
        </nav>
      </div>
</template>

<script>
  export default {
  name: 'nav-menu',
    props: {
      links: {
        type: Array,
        default: require
      }
    }
  }
</script>

<style lang="scss" scoped>
li {
  list-style-type: none;
}
  a {
    text-decoration: none;
    font-weight: 300;
    font-size: 18px;
    line-height: 21px;
    color: #E4E4E4;
  }
  .nav {
    &__items {
      display: flex;
    }
    &__item {
      margin-right: 145px;
    }
    &__item:last-child {
      margin-right: 0px;
    }
  }
</style>