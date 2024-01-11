<template>
  <header class="header">
    <nav class="header__nav container">

      <nuxt-link to="/" class="header__nav-logo"> 
        <!-- <img src="@/assets/images/logo.png" alt="Webstep">   -->
        webstep
      </nuxt-link>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  // background: #1B263B;
  color: white;
  padding: 20px 0;

  &__nav {
    &-logo {
      & img {
        width: 200px;
      }
    }
  }
}
</style>