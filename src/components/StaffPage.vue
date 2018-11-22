<template>
  <div class="main-wrapper">
      <!-- <navMenu></navMenu> -->
      <h1>STAFF PAGE</h1>
  </div>
</template>

<script>
import navMenu from './NavigationMenu'

export default {
  name: 'StaffPage',
  components: {
    navMenu
  },
  data () {
    return {
      mobileScreen: null
    }
  },
  mounted () {
    this.$nextTick(function () {
      window.addEventListener('resize', this.checkScreen)
      this.checkScreen()
    })
  },
  methods: {
    checkScreen () {
      (document.querySelector('.main-wrapper').getAttributeNode('mob-screen')) ? this.mobileScreen = true : this.mobileScreen = false
    }
  },
  beforeDestroy () {
    window.removeEventListener('resize', this.checkScreen)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
