<template>
  <div class="wrapper">
    <div class="logo">
      <nuxt-link to="/">
        <img
          src="@/assets/logo/decred-logo.png"
          alt="Decred logo"
          height="40"
          class="logo"
        />
      </nuxt-link>
    </div>
    <nav class="nav ml-5">
      <nuxt-link to="/basics">Decred Basics</nuxt-link>
      <nuxt-link to="/staking">How to Stake</nuxt-link>
      <nuxt-link to="/voting">How to Vote</nuxt-link>
      <nuxt-link to="/politeia">What is Politeia</nuxt-link>
    </nav>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({})
</script>

<style lang="scss" scoped>
@import '@/assets/_global';

$border-size: 2px;

.wrapper {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 70px;
  max-width: 1120px;
  margin: 0 auto;
  display: flex;
  flex-direction: row;
  align-items: center;
  // background-color: #fff;
  // border-bottom: thin solid #aaa;
}

.logo {
  // height: 40px;
  // border-bottom: $border-size solid transparent;
  margin-bottom: 2px;
}

.nav {
  display: flex;
  align-items: center;
  height: 100%;

  & > a {
    color: $color-primary-white;
    text-decoration: none;
    margin-right: 24px;
    border-bottom: $border-size solid transparent;
    padding-bottom: 2px;

    &:hover {
      border-bottom-color: $color-primary-white;
    }
  }
}
</style>
