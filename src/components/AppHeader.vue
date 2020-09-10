<template>
  <header class="header-wrapper">
    <h3 @click="homePage">
      HOME
    </h3>
    <h2 @click="toFaq">
      ?
    </h2>
  </header>
</template>

<script>
export default {
  name: 'appHeader',
  components: {
  },
  methods: {
    homePage () {
      this.$router.push({ name: 'Home' })
    },
    toFaq () {
      this.$router.push({ name: 'FAQ' })
    }
  }
}
</script>

<style scoped lang="less">
.header-wrapper {
  background-color: #003e81;
  height: 8vh;
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100vw;
  color: #fff;
  cursor: pointer;
}
</style>