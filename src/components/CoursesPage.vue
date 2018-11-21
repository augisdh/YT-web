<template>
  <div class="main-wrapper">
    <div class="courses-wrap">
      <div class="courses-head">
        <div class="courses-head-img d-flex-center">
          <div class="port-head-wrapper container margin-sides">
            <img src="./assets/coursespage/portfolio.jpg" alt="">
          </div>
        </div>
        <div class="clear-head-bottom"></div>
      </div>
      <div class="courses-content-wrap d-flex-center">
        <div class="container margin-sides">
          <div class="w-port-box shadow">
            <!-- <div class="w-port-content">
              <h4>
                <span></span>
              </h4>
            </div> -->
            <div class="w-port-line"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import navMenu from './NavigationMenu'

export default {
  name: 'CoursesPage',
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
.courses-wrap {
  background-color: #fafafa;
}

.courses-head {
  width: 100%;
}
  .courses-head-img {
    width: 100%;
    padding-top: 38.2%;
    background: url(./assets/coursespage/courses_head.jpg) no-repeat center;
    background-size: 100%;
  }
    .port-head-wrapper {
      position: relative;
    }
      .port-head-wrapper > img {
        display: block;
        width: 50%;
        position: absolute;
        bottom: -100px;
        right: 0;
        z-index: 5;
      }
  .clear-head-bottom {
    width: 100%;
    height: 50px;
    background: transparent;
  }

  .w-port-box {
    position: relative;
    width: 90%;
    height: 300px;
    background-color: #fff;
    margin-bottom: 100px;
  }

/* Lines, etc... */
.w-port-line {
  position: absolute;
  right: -100px;
  bottom: 0;
  width: 150px;
  height: 5px;
  background-color: #b046aa;
  margin-bottom: 50px;
}

/* @Media */
@media (max-width: 550px) {
  .port-head-wrapper > img {
    bottom: -50px;
  }
  .clear-head-bottom {
    height: 25px;
  }

  .w-port-box {
    margin-bottom: 50px;
  }

  /* Lines */
  .w-port-line {
    right: -25px;
    width: 75px;
    margin-bottom: 25px;
  }
}

</style>
