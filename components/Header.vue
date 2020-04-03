<template>
  <div class="nav_wrap">

    <div class="container">
      <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
          <a class="navbar-item" href="#">
            <img src="https://i.pinimg.com/originals/af/f5/78/aff5786664d1ef5b5384f99ee3e137b9.png" class="nav_logo">
          </a>
          <a class="navbar-item" href="#">
            ООО «Прогресс Агро»
          </a>

          <a role="button" :class="classesBurger" aria-label="menu" aria-expanded="false"
             data-target="navbarBasicExample" @click="toggleMenu">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>

        </div>

        <div id="navbarBasicExample" :class="classesNavbar">
          <div class="navbar-end">

            <a class="navbar-item" href="tel:79165555555">
              +7 916 268-81-87
            </a>

            <nuxt-link class="navbar-item" to="/">
              Главная
            </nuxt-link>

            <nuxt-link class="navbar-item" to="/about">
              О компании
            </nuxt-link>

            <nuxt-link class="navbar-item" to="/contacts">
              Контакты
            </nuxt-link>

          </div>
        </div>
      </nav>
    </div>

  </div>
</template>

<script>
export default {
  data(){
    return {
      isActive: false
    }
  },
  computed: {
    classesBurger (){

      return {
        'navbar-burger': true,
        'burger': true,
        'is-active': this.isActive
      }

    },
    classesNavbar (){

      return {
        'navbar-menu': true,
        'is-active': this.isActive
      }

    },

  },
  methods: {
    toggleMenu() {

      if(this.isActive){
        this.isActive = false
      } else {
        this.isActive = true
      }

    },
  }
}
</script>

<style lang="scss">

  .nav_wrap {
    padding: 1rem 1.5rem;
  }

  .nav_logo {
    height: 50px;
  }

</style>
