<template>
  <div class="doc-links">
    <router-link v-if="api" :to="`${$localePath}api/${api}`">API</router-link>
    <demo-link v-if="demo" :href="demo">Demo</demo-link>
  </div>
</template>

<script>
// 演示链接
export default {
  props: {
    api: String,
    demo: String
  }
}
</script>

<style lang="stylus" scoped>
.doc-links
  float right
  padding 5px 1em
  background-color #f7f7f7
  border-radius 2em
  box-shadow inset 0 0 2px rgba(0,0,0,.05)

  p + &
  div + &
    margin-top -3px

  h2 + &
    margin-top -2.4em

  > a
    margin-right 1em

    &:last-child
      margin-right 0
</style>

