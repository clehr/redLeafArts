<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <nuxt-link v-bind:to="'/'" class="navbar-item">
        <img src="~/assets/logo.png" width="112" height="28" />
      </nuxt-link>

      <a
        role="button"
        class="navbar-burger burger"
        aria-label="menu"
        aria-expanded="false"
        data-target="navbarBasicExample"
        v-on:click="showNav = !showNav"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="navbarBasicExample" class="navbar-menu" v-bind:class="{ 'is-active' : showNav }">
      <div class="navbar-start">
        <nuxt-link v-bind:to="'/'" class="navbar-item">Shop</nuxt-link>
        <nuxt-link v-bind:to="'/about'" class="navbar-item">About</nuxt-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      showNav: false
    };
  }
};
</script>