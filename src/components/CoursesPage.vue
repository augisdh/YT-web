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
            <div class="w-port-content">
              <h4>
                什么是作品集?
                <span>WHAT IS A PORTFOLIO?</span>
              </h4>
              <p class="p-text">
                对于艺术与设计专业的学生来说，作品集是艺术留学的核心，国外院校大都要求学生提交作品集，
                作品集的质量是学生艺术综合实力的展现，是国外院校决定是否录取的重要依据，优秀作品集还能为学生赢得高额奖学金。
                国外院校主要是通过考察学生独立的创意思想以及对生活与文化的独特见解和表现手法，
                择优录取有创新意识、创意灵感和艺术天赋的优秀学生。
              </p>
            </div>
            <div class="w-port-line"></div>
          </div>
          <div class="port-course-box">
            <div class="port-course-head">
              <h4>
                作品集课程
                <span>PORTFOLIO COURSES</span>
              </h4>
            </div>
            <div class="port-course-content-grid shadow">
              <div class="course-one">
                <img src="./assets/coursespage/courses_b/B2-1.jpg" alt="">
                <div class="sub-ctx">
                  <h3>期初评估</h3>
                </div>
              </div>
              <div class="course-two">
                <img src="./assets/coursespage/courses_b/B2-2.jpg" alt="">
                <div class="sub-ctx">
                  <h3>择校策略分析</h3>
                </div>
              </div>
              <div class="course-three">
                <img src="./assets/coursespage/courses_b/B2-3.jpg" alt="">
                <div class="sub-ctx">
                  <h3>课程规划定制</h3>
                </div>
              </div>
              <div class="course-four">
                <img src="./assets/coursespage/courses_b/B2-4.jpg" alt="">
                <div class="sub-ctx">
                  <h3>留学时间规划</h3>
                </div>
              </div>
              <div class="course-five">
                <img src="./assets/coursespage/courses_b/B2-5.jpg" alt="">
                <div class="sub-ctx">
                  <h3>Project-1</h3>
                </div>
              </div>
              <div class="course-six">
                <img src="./assets/coursespage/courses_b/B2-6.jpg" alt="">
                <div class="sub-ctx">
                  <h3>Project-2</h3>
                </div>
              </div>
              <div class="course-seven">
                <img src="./assets/coursespage/courses_b/B2-7.jpg" alt="">
                <div class="sub-ctx">
                  <h3>Project-3</h3>
                </div>
              </div>
              <div class="course-eight">
                <img src="./assets/coursespage/courses_b/B2-8.jpg" alt="">
                <div class="sub-ctx">
                  <h3>Project-4</h3>
                </div>
              </div>
            </div>
          </div>
          <div class="vip-prog-box">
            <div class="vip-prog-head">
              <h4>
                VIP增值项
                <span>VIP PROGRAMME</span>
              </h4>
            </div>
            <div class="vip-prog-content-grid shadow">
              <div class="prog-one">
                <img src="./assets/coursespage/course_c/B3-1.jpg" alt="">
                <div class="sub-ctx">
                  <h3>精英导师审核</h3>
                </div>
              </div>
              <div class="prog-two">
                <img src="./assets/coursespage/course_c/B3-2.jpg" alt="">
                <div class="sub-ctx">
                  <h3>专项排版定制</h3>
                </div>
              </div>
              <div class="prog-three">
                <img src="./assets/coursespage/course_c/B3-3.jpg" alt="">
                <div class="sub-ctx">
                  <h3>定向国家翻译</h3>
                </div>
              </div>
              <div class="prog-four">
                <img v-if="mobileScreen === false" src="./assets/coursespage/course_c/B3-4.jpg" alt="">
                <img v-if="mobileScreen === true" src="./assets/coursespage/course_c/B3-4_mobile.jpg" alt="">
                <div class="sub-ctx">
                  <h3>名校面试辅导</h3>
                </div>
              </div>
              <div class="prog-five">
                <img v-if="mobileScreen === false" src="./assets/coursespage/course_c/B3-5.jpg" alt="">
                <img v-if="mobileScreen === true" src="./assets/coursespage/course_c/B3-5_mobile.jpg" alt="">
                <div class="sub-ctx">
                  <h3>专项挑战题</h3>
                </div>
              </div>
              <div class="prog-six">
                <img src="./assets/coursespage/course_c/B3-6.jpg" alt="">
                <div class="sub-ctx">
                  <h3>文书申请</h3>
                </div>
              </div>
              <div class="prog-seven">
                <img src="./assets/coursespage/course_c/B3-7.jpg" alt="">
                <div class="sub-ctx">
                  <h3>院校跟踪</h3>
                </div>
              </div>
            </div>
          </div>
          <div class="b-course-box">
            <div class="b-course-head">
              <h4>
                破冰基础课
                <span>BASIC COURSES</span>
              </h4>
            </div>
            <div class="b-course-content-wrap">
              <div class="b-course-content">
                <div class="b-course shadow">
                  <div class="b-course-img">
                    <img src="./assets/coursespage/course_d/B4-1.jpg" alt="">
                  </div>
                  <div class="b-course-ctx">
                    <h3></h3>
                    <p></p>
                  </div>
                </div>
                <div class="b-course shadow">
                  <div class="b-course-img">
                    <img src="./assets/coursespage/course_d/B4-2.jpg" alt="">
                  </div>
                  <div class="b-course-ctx">
                    <h3></h3>
                    <p></p>
                  </div>
                </div>
              </div>
              <div class="b-course-content">
                <div class="b-course shadow">
                  <div class="b-course-img">
                    <img src="./assets/coursespage/course_d/B4-3.jpg" alt="">
                  </div>
                  <div class="b-course-ctx">
                    <h3></h3>
                    <p></p>
                  </div>
                </div>
                <div class="b-course shadow">
                  <div class="b-course-img">
                    <img src="./assets/coursespage/course_d/B4-4.jpg" alt="">
                  </div>
                  <div class="b-course-ctx">
                    <h3></h3>
                    <p></p>
                  </div>
                </div>
              </div>
            </div>
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

  .courses-content-wrap {
    height: auto;
  }
  .w-port-box {
    position: relative;
    width: 90%;
    height: auto;
    background-color: #fff;
    margin-bottom: 100px;
    padding: 50px 0;
  }
    .w-port-box .w-port-content {
      margin: 0 50px;
      text-align: left;
    }
      .w-port-content > h4,
      .port-course-head > h4,
      .vip-prog-head > h4,
      .b-course-head h4 {
        margin: 0 0 50px 0;
        font-size: 2rem;
      }
        .w-port-content > h4 span,
        .port-course-head > h4 span,
        .vip-prog-head > h4 span,
        .b-course-head h4 span {
          display: block;
          font-size: 1rem;
        }
      .w-port-content .p-text {
        margin: 0 0 50px 0;
      }

    .port-course-head {
      margin-bottom: 50px;
    }

    /* Portfolio courses */
    .port-course-content-grid,
    .vip-prog-content-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      grid-template-rows: repeat(2, auto);
      width: 100%;
      margin-bottom: 100px;
    }
      .port-course-content-grid > div,
      .vip-prog-content-grid > div {
        position: relative;
      }
      /* Grid course position */
      .course-one {
        grid-column: 1/3;
        grid-row: 1;
      }
      .course-two {
        grid-column: 3;
        grid-row: 1;
      }
      .course-three {
        grid-column: 4;
        grid-row: 1;
      }
      .course-four {
        grid-column: 5;
        grid-row: 1/3;
      }
      .course-five {
        grid-column: 1;
        grid-row: 2;
      }
      .course-six {
        grid-column: 2;
        grid-row: 2;
      }
      .course-seven {
        grid-column: 3;
        grid-row: 2;
      }
      .course-eight {
        grid-column: 4;
        grid-row: 2;
      }
        .port-course-content-grid img,
        .vip-prog-content-grid img {
          display: block;
          width: 100%;
        }
        .port-course-content-grid .sub-ctx,
        .vip-prog-content-grid .sub-ctx {
          position: absolute;
          top: 25px;
          left: 25px;
        }
          .sub-ctx > h3 {
            margin: 0;
            font-size: 18px;
          }

    /* VIP programme */
    .prog-one {
      grid-column: 1;
      grid-row: 1/3;
    }
    .prog-two {
      grid-column: 2;
      grid-row: 1;
    }
    .prog-three {
      grid-column: 3;
      grid-row: 1;
    }
    .prog-four {
      grid-column: 4/6;
      grid-row: 1;
    }
    .prog-five {
      grid-column: 2/4;
      grid-row: 2;
    }
    .prog-six {
      grid-column: 4;
      grid-row: 2;
    }
    .prog-seven {
      grid-column: 5;
      grid-row: 2;
    }

  /* BASIC COURSES */
  .b-course-content-wrap {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    flex-wrap: wrap;
    width: 100%;
    margin-bottom: 75px;
  }
    .b-course-content {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    }
    .b-course-content {
      margin-bottom: 25px;
    }
      .b-course:first-child {
        margin-right: 25px;
      }
        .b-course-img > img {
          display: block;
          width: 100%;
        }

      .b-course-ctx {
        height: 200px;
        background-color: #b046aa;
      }
        .b-course-ctx > h3 {
          margin: 0;
        }
        .b-course-ctx > p {
          margin: 0;
        }

/* Lines, etc... */
.w-port-line {
  position: absolute;
  right: -100px;
  bottom: 50px;
  width: 150px;
  height: 5px;
  background-color: #b046aa;
}

/* @Media */
@media (max-width: 800px) {
  .port-course-content-grid,
  .vip-prog-content-grid {
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(4, auto);
  }
  /* Grid course position */
  .course-three {
    grid-column: 1;
    grid-row: 2;
  }
  .course-four {
    grid-column: 2;
    grid-row: 2/4;
  }
  .course-five {
    grid-column: 3;
    grid-row: 2;
  }
  .course-six {
    grid-column: 1;
    grid-row: 3;
  }
  .course-seven {
    grid-column: 3;
    grid-row: 3;
  }
  .course-eight {
    grid-column: 2;
    grid-row: 4;
  }
  /* VIP programme */
  .prog-four {
    grid-column: 2/4;
    grid-row: 2;
  }
  .prog-five {
    grid-column: 1/3;
    grid-row: 3;
  }
  .prog-six {
    grid-column: 3;
    grid-row: 3;
  }
  .prog-seven {
    grid-column: 2;
    grid-row: 4;
  }
}

@media (max-width: 550px) {
  .port-head-wrapper > img {
    bottom: -50px;
  }
  .clear-head-bottom {
    height: 25px;
  }

  .w-port-box {
    margin-bottom: 50px;
    padding: 25px 0;
  }
    .w-port-box .w-port-content {
      margin: 0 25px;
    }
      .w-port-content > h4,
      .port-course-head > h4,
      .vip-prog-head > h4,
      .b-course-head h4 {
        margin: 0 0 25px 0;
      }
      .w-port-content > h4 {
        margin-top: 25px;
      }
    .w-port-content .p-text {
      margin: 0 0 25px 0;
    }

  .port-course-head {
    margin-bottom: 25px;
  }

  .port-course-content-grid {
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(5, auto);
    margin-bottom: 50px;
  }
  /* Grid course position */
  .course-two {
    grid-column: 1;
    grid-row: 2;
  }
  .course-three {
    grid-column: 2;
    grid-row: 2;
  }
  .course-four {
    grid-column: 1;
    grid-row: 3/5;
  }
  .course-five {
    grid-column: 2;
    grid-row: 3;
  }
  .course-six {
    grid-column: 2;
    grid-row: 4;
  }
  .course-seven {
    grid-column: 1;
    grid-row: 5;
  }
  .course-eight {
    grid-column: 2;
    grid-row: 5;
  }
    .port-course-content-grid .sub-ctx,
    .vip-prog-content-grid .sub-ctx {
      top: 10px;
      left: 10px;
    }

  .vip-prog-content-grid {
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(4, auto);
    margin-bottom: 50px;
  }
  /* VIP programme */
  .prog-three {
    grid-column: 2;
    grid-row: 2;
  }
  .prog-four {
    grid-column: 2;
    grid-row: 3;
  }
  .prog-five {
    grid-column: 1;
    grid-row: 3;
  }
  .prog-six {
    grid-column: 1;
    grid-row: 4;
  }

  /* BASIC COURSES */
  .b-course-content-wrap {
    margin-bottom: 25px;
  }
    .b-course:first-child {
      margin-right: 12.5px;
    }

  /* Lines */
  .w-port-line {
    right: -25px;
    width: 75px;
    bottom: 25px;
  }
}

</style>
