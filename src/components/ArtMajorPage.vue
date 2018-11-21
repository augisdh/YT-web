<template>
  <div class="main-wrapper">
      <!-- <navMenu></navMenu> -->
      <h1>ART MAJOR PAGE</h1>
  </div>
</template>

<script>
import navMenu from './NavigationMenu'

export default {
  name: 'ArtMajorPage',
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
    checkScreen (event) {
      (document.querySelector('.main-wrapper').attributes[2]) ? this.mobileScreen = true : this.mobileScreen = false
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
