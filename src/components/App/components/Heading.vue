<template lang='pug'>
  .heading
    router-link.name(to='/' tag='div').
      codeams
    transition(name='fade')
      span.ocupation(v-if='$route.name === "Portfolio"').
        passionated front-ender
</template>

<style lang='scss'>
  .heading {
    z-index: 2;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 70px;
    text-align: center;
    border-bottom: 3px solid darken(#202740, 5%);
    background-color: #202740;

    @include breakpoint(large) {
      width: auto;
      padding: 40px 0 40px 70px;
      text-align: left;
      border: none;
      background-color: transparent;
    }

    .name {
      font-size: 24px;
      font-weight: 500;
      letter-spacing: -1.16px;
      cursor: pointer;
    }

    .ocupation {
      font-size: 18px;
      letter-spacing: -0.12px;
      cursor: default;
    }
  }
</style>
