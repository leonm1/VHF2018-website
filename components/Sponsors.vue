<template>
  <div />
</template>


<style lang="scss">
@import "~assets/scss/variables.scss";
.sponsor-row {
  text-align: center;
  img {
    padding: 10px;
    vertical-align: middle;
    @media (min-width: $break-m) {
      padding: 15px;
    }
    @media (min-width: $break-l) {
      padding: 20px;
    }
  }
  &.tier-1 {
    img {
      width: 100%;
      max-width: 600px;
    }
  }
  &.tier-2 {
    img {
      width: 50%;
      max-width: 360px;
    }
  }
  &.tier-3 {
    img {
      width: 33.333%;
      height: auto;
    }
  }
}
</style>
