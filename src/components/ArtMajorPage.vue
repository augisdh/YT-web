<template>
  <div class="main-wrapper">
    <div class="disc-wrap">
      <div class="disc-head">
        <img v-if="mobileScreen === false" src="./assets/disciplinespage/pattern_bg.jpg" alt="">
        <img v-if="mobileScreen === true" src="./assets/disciplinespage/pattern_bg_mobile.jpg" alt="">
      </div>
      <div class="disc-content-wrap d-flex-center">
        <div class="container margin-sides">
          <div class="expl-sub-wrap">
            <div class="expl-sub-box shadow">
              <div class="expl-sub-content">
                <h4>
                  艺术专业
                  <span>EXPLORE SUBJECTS</span>
                </h4>
                <p class="p-text">
                  欧美顶级院校专业基础课程完美呈现，针对创意思维的能力进行强化突击训练。
                  洋桃独家研发， 整个启蒙单元在不耗费过多作品集准备时间的前提下，以跨专业的项目实践为载体，
                  全程一对一 辅导，帮助学员切实掌握顶尖设计师必备的思维方法，及空间抽取、叙事表达、
                  同感联想、解构 意识、高语言重塑等进阶设计思维技巧。
                </p>
              </div>
              <div class="purple-line"></div>
            </div>
          </div>
          <div class="disc-sub-content-wrap">
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
            <div class="disc-sub-box shadow"></div>
          </div>
        </div>
      </div>
    </div>
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
      window.addEventListener('resize', this.changeExplDivHeight)
      this.changeExplDivHeight()
    })
  },
  methods: {
    checkScreen () {
      (document.querySelector('.main-wrapper').getAttributeNode('mob-screen')) ? this.mobileScreen = true : this.mobileScreen = false
    },
    changeExplDivHeight () {
      (window.innerWidth < 1150) ? document.querySelector('.expl-sub-wrap').style.height = `${document.querySelector('.expl-sub-box').offsetTop + document.querySelector('.expl-sub-box').offsetHeight}px` : document.querySelector('.expl-sub-wrap').removeAttribute('style')
    }
  },
  beforeDestroy () {
    window.removeEventListener('resize', this.checkScreen)
    window.removeEventListener('resize', this.changeExplDivHeight)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.disc-wrap {
  background-color: #fafafa;
}

.disc-head {
  width: 100%;
}
  .disc-head > img {
    display: block;
    width: 100%;
  }

  .expl-sub-wrap {
    position: relative;
    margin-bottom: 50px;
  }
    .expl-sub-box {
      position: absolute;
      top: -375px;
      width: 100%;
      background-color: #fff;
    }
      .expl-sub-content {
        margin: 50px;
        text-align: left;
      }
        .expl-sub-content > h4 {
          margin: 0 0 50px 0;
          font-size: 2rem;
        }
          .expl-sub-content > h4 span {
            display: block;
            font-size: 1rem;
          }
        .expl-sub-content .p-text {
          margin: 0;
        }

  .disc-sub-content-wrap {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    margin-bottom: 100px;
  }
    .disc-sub-box {
      max-width: 487.5px;
      width: 100%;
      height: 500px;
      background-color: #fff;
      margin-bottom: 50px;
    }
    .disc-sub-box:nth-child(odd) {
      margin-right: 12.5px;
    }
    .disc-sub-box:nth-child(even) {
      margin-left: 12.5px;
    }

/* Lines, etc */
.purple-line {
  width: 100px;
  height: 5px;
  float: right;
  margin: 0 50px 45px 0;
  background-color: #ae4ea9;
}
/* @Media */
@media (max-width: 1049px) {
  .expl-sub-box {
    top: -125px;
  }
  .disc-sub-box:nth-child(odd),
  .disc-sub-box:nth-child(even) {
    margin-left: 12.5px;
    margin-right: 12.5px;
  }
}

@media (max-width: 1024px) {
  .disc-sub-box:nth-child(odd),
  .disc-sub-box:nth-child(even) {
    margin-left: 0;
    margin-right: 0;
  }
}

@media (max-width: 550px) {
  .expl-sub-wrap {
    margin-bottom: 25px;
  }
    .expl-sub-box {
      top: -25px;
    }
      .expl-sub-content {
        margin: 25px;
      }
        .expl-sub-content > h4 {
          margin: 0 0 25px 0;
        }

  .disc-sub-content-wrap {
    margin-bottom: 50px;
  }
    .disc-sub-box {
      margin-bottom: 25px;
    }

/* Lines, etc */
  .purple-line {
    width: 50px;
    margin: 0 25px 20px 0;
  }
}
</style>
