<template>
  <div class="main-wrapper">
    <div class="intro-wrap d-flex-center">
      <div class="intro-ctx-wrap container margin-sides">
        <div class="intro-ctx-box">

        </div>
      </div>
    </div>
    <div class="disciplines-wrap d-flex-center">
      <!-- <div class="disciplines-grid container margin-sides shadow">
        <div class="industrial-d">
          <img src="./assets/homepage/disciplines/industrial.jpg" alt="">
          <div class="sub-ctx">
            <h3>工业设计</h3>
            <h5>Industrial Design</h5>
          </div>
        </div>
        <div class="film">
          <img src="./assets/homepage/disciplines/filming.jpg" alt="">
          <div class="sub-ctx">
            <h3>影视制作</h3>
            <h5>Film</h5>
          </div>
        </div>
        <div class="arts">
          <img src="./assets/homepage/disciplines/fine_arts.jpg" alt="">
          <div class="sub-ctx">
            <h3>纯艺术</h3>
            <h5>Fine Arts</h5>
          </div>
        </div>
        <div class="fashion-d">
          <img src="./assets/homepage/disciplines/fashion_design.jpg" alt="">
          <div class="sub-ctx">
            <h3>服装设计 &<br> 时尚管理</h3>
            <h5>Fashion Design<br> & Management</h5>
          </div>
        </div>
        <div class="interior-d">
          <img src="./assets/homepage/disciplines/interior_design.jpg" alt="">
          <div class="sub-ctx">
            <h3>室内设计</h3>
            <h5>Interior Design</h5>
          </div>
        </div>
        <div class="jewellery-d">
          <img src="./assets/homepage/disciplines/jewellery_design.jpg" alt="">
          <div class="sub-ctx">
            <h3>珠宝设计</h3>
            <h5>Jewellery Design</h5>
          </div>
        </div>
        <div class="graphic-d">
          <img v-if="mobileScreen === false" src="./assets/homepage/disciplines/graphic_design.jpg" alt="">
          <img v-if="mobileScreen === true" src="./assets/homepage/disciplines/graphic_design_sm.jpg" alt="">
          <div class="sub-ctx">
            <h3>平麵设计</h3>
            <h5>Graphic Design</h5>
          </div>
        </div>
        <div class="anim">
          <img src="./assets/homepage/disciplines/animation.jpg" alt="">
          <div class="sub-ctx">
            <h3>動画</h3>
            <h5>Animation</h5>
          </div>
        </div>
        <div class="photography">
          <img src="./assets/homepage/disciplines/fotography.jpg" alt="">
          <div class="sub-ctx">
            <h3>摄影</h3>
            <h5>Photography</h5>
          </div>
        </div>
        <div class="interaction-d">
          <img src="./assets/homepage/disciplines/interactive_design.jpg" alt="">
          <div class="sub-ctx">
            <h3>交互设计</h3>
            <h5>Interaction Design</h5>
          </div>
        </div>
        <div class="visual-c">
          <img src="./assets/homepage/disciplines/visual_communication.jpg" alt="">
          <div class="sub-ctx">
            <h3>视觉传达</h3>
            <h5>Visual Communication</h5>
          </div>
        </div>
      </div> -->
    </div>
    <div class="about-pages-one-wrap d-flex-center">
      <div class="about-pages-section container margin-sides">
        <div class="section-box shadow">
          <div class="portfolio-box-one">
            <p class="p-text">
              洋桃YoungTalent，一个由多位海归精英设计师集结力量共同创立的国际艺术设计联盟体，始创于中国上海，专注于海内外的设计师孵化
              、产业合作链建立；同时，也是一个师资强大的国际艺术咨询中心，致力于最专业的艺术家与设计师养成计划、作品集指导、艺术留学规划，
              位于上海市南京西路地段。艺术社区的形态摆脱定式束缚，是全新艺术设计方式的转变。
            </p>
          </div>
          <div class="portfolio-box-one">
            <h1>
              BUILD YOUR PORTFOLIO, <br> JOIN OUR COMMUNITY...
            </h1>
            <div class="portfolio-arrow"></div>
          </div>
        </div>
        <div class="section-box d-flex-staff shadow">
          <div class="staff-box">
            <img src="./assets/homepage/staff/becca-homepage.jpg" alt="">
            <img src="./assets/homepage/staff/freddie-homepage.jpg" alt="">
            <img src="./assets/homepage/staff/cassie-homepage.jpg" alt="">
          </div>
          <div class="staff-box-ctx">
            <p class="p-text">
              <span>曾经漂洋过海，而今桃李满天。</span><br>
              CULTIVATING TALENTS ACROSS <br>
              THE WORLD, ACHIEVING THE <br>
              BEST RESULTS.
            </p>
            <div class="portfolio-arrow"></div>
          </div>
        </div>
        <div class="section-box shadow">
          <div class="content-box">
            <div class="content-heading-box">
              <h4>
                <span>合作院校</span>
                UNIVERSITY PARTNERS
              </h4>
            </div>
            <div class="univer-img-box">
              <div class="univer-pic"><img src="./assets/homepage/universities/E3-9-homepage.png" alt=""></div>
              <div class="univer-pic"><img src="./assets/homepage/universities/E-6-homepage.png" alt=""></div>
              <div class="univer-pic"><img src="./assets/homepage/universities/E-1-homepage.png" alt=""></div>
              <div class="univer-pic"><img src="./assets/homepage/universities/E2-1-homepage.png" alt=""></div>
              <div class="univer-pic"><img src="./assets/homepage/universities/E3-8-homepage.png" alt=""></div>
              <div class="univer-pic"><img src="./assets/homepage/universities/E-7-homepage.png" alt=""></div>
              <div class="univer-pic"><img src="./assets/homepage/universities/E2-2-homepage.png" alt=""></div>
              <div class="portfolio-arrow"></div>
            </div>
          </div>
        </div>
        <div class="section-box shadow">
          <div class="content-box">
            <div class="content-heading-box">
              <h4>
                <span>學生案例</span>
                STUDENT CASES
              </h4>
            </div>
            <div class="stud-case-p">
              <p class="p-text">
                在艺术留学方面，洋桃和许多世界顶级艺术院校 （如： CSM中央圣马丁、PARSONS帕森斯、RCA皇家艺术学院、RISD罗德岛设计学院）
                建立深度合作关系，双向输送艺术设计方面的顶尖人才。作为设计师联盟，我们为优秀的人才提供最广阔的发展平台。
              </p>
            </div>
            <div class="horizontal-line"></div>
          </div>
        </div>
      </div>
    </div>
    <div class="about-pages-two-wrap d-flex-center">
      <div class="about-pages-section container margin-sides">
        <div class="section-main-box">
          <div class="content-heading-box">
              <h4>
                <span>本科生</span>
                UNDERGRADUATE STUDENT CASES
              </h4>
          </div>
          <div class="stu-case-box shadow">
            <div class="student-ctx">
              <div class="student-img">
                <img src="./assets/homepage/studentcase/underg/undergraduate_profile_1.jpg" alt="">
              </div>
              <div class="student-p">
                <p class="p-text">
                  <span>
                    王同学<br>
                    电影电视 / 视觉传达
                  </span>
                  香港演艺学院
                  伦敦艺术大学
                  爱丁堡大学
                  等6所大学
                </p>
              </div>
            </div>
            <div class="plus-simb">&#43;</div>
            <div class="student-project">
              <div class="img-wrap">
                <img
                  v-if="mobileScreen === false"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/porfolio_small1.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_portfolio_large1.jpg"
                  alt="">
                <img
                  v-if="mobileScreen === true"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/porfolio_small1_mobile.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_portfolio_large1.jpg"
                  alt="">
              </div>
              <div class="img-wrap">
                <img
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/undergraduate_offer1.1.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_offer_large1.jpg"
                  alt="">
              </div>
            </div>
          </div>
          <div class="stu-case-box shadow">
            <div class="student-ctx">
              <div class="student-img">
                <img src="./assets/homepage/studentcase/underg/undergraduate_profile_2.jpg" alt="">
              </div>
              <div class="student-p">
                <p class="p-text">
                  <span>
                    叶同学<br>
                    纯艺术
                  </span>
                  马里兰艺术学院
                  普瑞特艺术学院
                  纽约视觉艺术学院
                  等5所大学
                </p>
              </div>
            </div>
            <div class="plus-simb">&#43;</div>
            <div class="student-project">
              <div class="img-wrap">
                <img
                  v-if="mobileScreen === false"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/portfolio_small2.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_portfolio_large2.jpg"
                  alt="">
                <img
                  v-if="mobileScreen === true"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/portfolio_small2_mobile.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_portfolio_large2.jpg"
                  alt="">
              </div>
              <div class="img-wrap">
                <img
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/undergraduate_offer2.1.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_offer_large2.jpg"
                  alt="">
              </div>
            </div>
          </div>
          <div class="stu-case-box shadow">
            <div class="student-ctx">
              <div class="student-img">
                <img src="./assets/homepage/studentcase/underg/undergraduate_profile_3.jpg" alt="">
              </div>
              <div class="student-p">
                <p class="p-text">
                  <span>
                    林同学<br>
                    摄影
                  </span>
                  伦敦艺术大学
                  布莱顿大学
                  圣安德鲁斯剑桥学院
                </p>
              </div>
            </div>
            <div class="plus-simb">&#43;</div>
            <div class="student-project">
              <div class="img-wrap">
                <img
                  v-if="mobileScreen === false"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/portfolio_small3.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_portfolio_large3.jpg"
                  alt="">
                <img
                  v-if="mobileScreen === true"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/portfolio_small3_mobile.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_portfolio_large3.jpg"
                  alt="">
              </div>
              <div class="img-wrap">
                <img
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/underg/undergraduate_offer3.1.jpg"
                  data-enlarge="static/enlarge/underg/undergraduate_offer_large3.jpg"
                  alt="">
              </div>
            </div>
          </div>
        </div>
        <div class="section-main-box">
          <div class="content-heading-box">
              <h4>
                <span>研究生</span>
                POSTGRADUATE STUDENT CASES
              </h4>
          </div>
          <div class="stu-case-box shadow">
            <div class="student-ctx">
              <div class="student-img">
                <img src="./assets/homepage/studentcase/postg/postgraduate_profile_1.jpg" alt="">
              </div>
              <div class="student-p">
                <p class="p-text">
                  <span>
                    朱同学<br>
                    工业设计
                  </span>
                  中央圣马丁艺术与设计学院
                </p>
              </div>
            </div>
            <div class="plus-simb">&#43;</div>
            <div class="student-project">
              <div class="img-wrap">
                <img
                  v-if="mobileScreen === false"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/portfolio_small4.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_portfolio_large1.jpg"
                  alt="">
                <img
                  v-if="mobileScreen === true"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/portfolio_small4_mobile.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_portfolio_large1.jpg"
                  alt="">
              </div>
              <div class="img-wrap">
                <img
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/postgraduate_offer1.1.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_offer_large1.jpg"
                  alt="">
              </div>
            </div>
          </div>
          <div class="stu-case-box shadow">
            <div class="student-ctx">
              <div class="student-img">
                <img src="./assets/homepage/studentcase/postg/postgraduate_profile_2.jpg" alt="">
              </div>
              <div class="student-p">
                <p class="p-text">
                  <span>
                    李同学<br>
                    视觉传达
                  </span>
                  德国魏玛包豪斯大学
                </p>
              </div>
            </div>
            <div class="plus-simb">&#43;</div>
            <div class="student-project">
              <div class="img-wrap">
                <img
                  v-if="mobileScreen === false"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/portfolio_small5.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_portfolio_large2.jpg"
                  alt="">
                <img
                  v-if="mobileScreen === true"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/portfolio_small5_mobile.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_portfolio_large2.jpg"
                  alt="">
              </div>
              <div class="img-wrap">
                <img
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/postgraduate_offer2.1.jpg" alt=""
                  data-enlarge="static/enlarge/postg/postgraduate_offer_large2.jpg">
              </div>
            </div>
          </div>
          <div class="stu-case-box mb-0 shadow">
            <div class="student-ctx">
              <div class="student-img">
                <img src="./assets/homepage/studentcase/postg/postgraduate_profile_3.jpg" alt="">
              </div>
              <div class="student-p">
                <p class="p-text">
                  <span>
                    张同学<br>
                    交互设计
                  </span>
                  伦敦艺术大学
                  拉夫堡大学
                </p>
              </div>
            </div>
            <div class="plus-simb">&#43;</div>
            <div class="student-project">
              <div class="img-wrap">
                <img
                  v-if="mobileScreen === false"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/portfolio_small6.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_portfolio_large3.jpg"
                  alt="">
                <img
                  v-if="mobileScreen === true"
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/portfolio_small6_mobile.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_portfolio_large3.jpg"
                  alt="">
              </div>
              <div class="img-wrap">
                <img
                  @click="getEnlargeImg"
                  src="./assets/homepage/studentcase/postg/postgraduate_offer3.1.jpg"
                  data-enlarge="static/enlarge/postg/postgraduate_offer_large3.jpg"
                  alt="">
              </div>
            </div>
          </div>
          <div class="case-b-txt-wrapper">
            <p class="p-text">
              联系我们，了解更多案例
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- Modal BOX -->
    <div id="modal-box" class="modal" :class="{'display-f': modalBoxActive === true, 'display-n': modalBoxActive !== true}">
      <span class="close" @click="closeModalBox">&times;</span>
      <div class="margin-sides">
        <img class="modal-img" :src="enlargeImg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
import navMenu from './NavigationMenu'

export default {
  name: 'HomePage',
  components: {
    navMenu
  },
  data () {
    return {
      mobileScreen: null,
      modalBoxActive: Boolean,
      enlargeImg: String
    }
  },
  mounted () {
    this.$nextTick(function () {
      window.addEventListener('resize', this.getWindowWidth)
      this.getWindowWidth()
    })
  },
  methods: {
    getWindowWidth (event) {
      const windowWidth = document.documentElement.clientWidth;
      (windowWidth <= 550) ? this.mobileScreen = true : this.mobileScreen = false
    },
    getEnlargeImg (event) {
      this.enlargeImg = event.target.dataset.enlarge
      this.modalBoxActive = true
    },
    closeModalBox () {
      this.modalBoxActive = !this.modalBoxActive
    }
  },
  beforeDestroy () {
    window.removeEventListener('resize', this.getWindowWidth)
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* Intro SCROLL DOWN */
.intro-wrap {
  width: 100%;
  height: 100vh;
  background: url(./assets/homepage/topcover/hp_cover.jpg) no-repeat center;
  background-size: cover;
}
  .intro-ctx-wrap {
    display: flex;
    justify-content: center;
    align-items: center;
  }
    .intro-ctx-box {
      width: 100%;
      height: 100%;
      background: plum;
    }

/* Disciplines GRID */
.disciplines-wrap {
  padding: 150px 0 100px 0;
  background: #b046aa;
}
  .disciplines-grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(3, auto);
    background: #fff;
  }

  .disciplines-grid > div {
    position: relative;
    height: 100%;
  }
  .disciplines-grid > div::after {
    display: none;
    content: '';
    position: absolute;
    right: 25px;
    bottom: 25px;
    width: 22px;
    height: 22px;
    background: url(./assets/contactform/arrow-corner.png) no-repeat center;
  }
    .disciplines-grid > div img {
      width: 100%;
      height: 100%;
    }
    .sub-ctx {
      position: absolute;
      top: 25px;
      left: 25px;
      text-align: left;
    }
      .sub-ctx > h3,
      .sub-ctx > h5 {
        margin: 0;
      }
      .sub-ctx > h3 {
        font-size: 18px;
      }
      .sub-ctx > h5 {
        font-size: 14px;
      }

  .disciplines-grid > div:hover {
    opacity: 0.95;
    cursor: pointer;
  }
  .disciplines-grid > div:hover:after {
    display: block;
  }
  .disciplines-grid > div:hover h3 {
    color: #000;
  }
  .disciplines-grid > div:hover h5 {
    color: #23e8be;
  }

  .industrial-d {
    grid-column: 1;
    grid-row: 1;
  }
  .film {
    grid-column: 2;
    grid-row: 1;
  }
  .arts {
    grid-column: 3;
    grid-row: 1;
  }
  .fashion-d {
    grid-column: 4;
    grid-row: 1/3;
  }
  .interior-d {
    grid-column: 5;
    grid-row: 1;
  }
  .jewellery-d {
    grid-column: 1/3;
    grid-row: 2;
  }
  .graphic-d {
    grid-column: 3;
    grid-row: 2/4;
  }
  .anim {
    grid-column: 5;
    grid-row: 2;
  }
  .photography {
    grid-column: 1;
    grid-row: 3;
  }
  .interaction-d {
    grid-column: 2;
    grid-row: 3;
  }
  .visual-c {
    grid-column: 4/6;
    grid-row: 3;
  }

/* About section (univer, students...) */
.about-pages-one-wrap {
  width: 100%;
  background: linear-gradient(to bottom, #b046aa 200px, #fafafa 200px, #fafafa 100%);
}

  .about-pages-section {
    display: flex;
    flex-direction: column;
  }
    .section-box,
    .section-main-box {
      width: 100%;
      margin-bottom: 100px;
    }
    .section-box {
      background: #fff;
    }
    .section-box:last-child {
      margin-bottom: 0px;
    }

.about-pages-two-wrap {
  width: 100%;
  background: linear-gradient(to top, #b046aa 250px, #fafafa 250px, #fafafa 100%);
}
  .section-main-box {
    background: transparent;
  }
  .section-main-box:first-child {
    margin-top: 100px;
    margin-bottom: 50px;
  }

  .portfolio-box-one {
    position: relative;
    margin: 50px;
    text-align: left;
  }
    .portfolio-box-one h1 {
      display: inline-block;
      color: #fccd0f;
      margin: 0 30px 0 0;
      font-size: 2rem;
    }

  .d-flex-staff {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
  }
  .staff-box {
    display: inline-block;
    max-width: 600px;
    width: 100%;
  }
    .staff-box img {
      display: block;
      float: left;
      width: calc(100%/3);
    }

  .staff-box-ctx {
    position: relative;
    margin: 50px;
    text-align: left;
    max-width: 300px;
    width: 100%;
  }
    .staff-box-ctx p {
      display: inline-block;
      margin: 0 30px 0 0;
      width: 100%;
    }
    .staff-box-ctx p > span {
      display: inline-block;
      padding-bottom: 5px;
    }

  .content-box {
    height: 100%;
    margin: 50px;
  }
    .content-heading-box {
      width: 100%;
    }
      .content-heading-box h4 {
        font-size: 1rem;
        margin: 25px 0 25px 0;
      }
        .content-heading-box h4 span {
          display: block;
          width: 100%;
          font-size: 2rem;
        }

    .univer-img-box {
      position: relative;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }
      .univer-img-box .univer-pic {
        margin-top: 25px;
      }
      .univer-img-box .univer-pic:nth-child(7) {
        margin-right: 69px;
      }
      .univer-img-box .portfolio-arrow {
        bottom: 12px;
      }

    .stud-case-p {
      text-align: left;
      margin-top: 50px;
    }

  .section-main-box .content-heading-box h4 {
    margin: 0;
  }

  .stu-case-box {
    position: relative;
    display: flex;
    flex-direction: row;
    background: #fff;
    margin: 50px 0;
  }
    .student-ctx {
      margin: 25px;
      max-width: 350px;
      min-width: 100px;
      width: 100%;
      height: 150px;
      display: flex;
      flex-direction: row;
      align-self: center;
    }
      .student-img img {
        width: 100%;
      }
      .student-p {
        margin: 0 25px;
        max-width: 150px;
        text-align: left;
      }
        .student-p span {
          display: block;
          margin-bottom: 10px;
        }

    .student-project {
      display: flex;
      flex-direction: row;
      cursor: pointer;
      width: 100%;
    }
      .student-project .img-wrap:first-child {
        width: 100%;
      }
      .student-project .img-wrap:last-child {
        width: 50%;
      }
        .student-project .img-wrap img {
          display: block;
          width: 100%;
        }

  .case-b-txt-wrapper {
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: flex-end;
  }
    .case-b-txt-wrapper > .p-text {
      margin: 0;
      color: #fff;
    }

/* Arrow, lines, symbols */
.portfolio-arrow {
  position: absolute;
  right: 0;
  bottom: 5px;
  width: 19px;
  height: 30px;
  background: url(./assets/contactform/arrow-right.png) no-repeat center;
  cursor: pointer;
}
.horizontal-line {
  margin: auto;
  margin-top: 50px;
  width: 100px;
  height: 5px;
  background: #fccd0f;
}
.plus-simb {
  position: absolute;
  top: 70px;
  right: 182px;
  font-size: 60px;
  color: #23e8be;
}

/* Modal BOX */
.modal {
  justify-content: center;
  align-items: center;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.4);
}
  .modal-img {
    display: block;
    width: 100%;
  }

  .close {
    position: absolute;
    top: 15px;
    right: 35px;
    color: #f1f1f1;
    font-size: 40px;
    font-weight: bold;
    transition: 0.3s;
    cursor: pointer;
  }
  .close:hover,
  .close:focus {
      color: #bbb;
  }

/* @Media */
@media (max-width: 1049px) {
  .d-flex-staff {
    all: none;
  }
  .staff-box {
    max-width: unset;
  }
  .staff-box-ctx {
    max-width: unset;
  }
  .stu-case-box {
    flex-direction: column;
    flex: 1 1 30%;

  }
  .plus-simb {
    top: 167px;
    right: 50%;
    transform: translateX(18px)
  }
}

@media (max-width: 800px) {
  .disciplines-grid {
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(5, auto);
  }

  .fashion-d {
    grid-column: 1;
    grid-row: 4/6;
  }
  .interior-d {
    grid-column: 2;
    grid-row: 4;
  }
  .anim {
    grid-column: 3;
    grid-row: 4;
  }
  .visual-c {
    grid-column: 2/4;
    grid-row: 5;
  }
}

@media (max-width: 550px){
  .disciplines-wrap {
    padding: 75px 0 50px 0;
  }
  .disciplines-grid {
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(7, auto);
  }
    .disciplines-grid > div::after {
      right: 10px;
      bottom: 10px;
    }
    .sub-ctx {
      top: 10px;
      left: 10px;
    }

  .arts {
    grid-column: 2;
    grid-row: 4;
  }
  .fashion-d {
    grid-row: 5/7;
  }
  .interior-d {
    grid-row: 5;
  }
  .graphic-d {
    grid-column: 1;
    grid-row: 4;
  }
  .anim {
    grid-column: 2;
    grid-row: 6;
  }
  .visual-c {
    grid-column: 1/3;
    grid-row: 7;
  }

  .about-pages-one-wrap {
    background: linear-gradient(to bottom, #b046aa 75px, #fafafa 75px, #fafafa 100%);
  }
    .portfolio-box-one {
      margin: 25px;
    }

  .about-pages-two-wrap {
    background: linear-gradient(to top, #b046aa 150px, #fafafa 150px, #fafafa 100%);
  }
    .section-box,
    .section-main-box {
      margin-bottom: 50px;
    }
    .section-main-box:first-child {
      margin-top: 50px;
    }

  .staff-box-ctx {
    margin: 25px;
  }
    .staff-box-ctx p {
      margin: 0 30px 0 0;
    }

  .content-box {
    margin: 25px;
  }
    .univer-img-box .univer-pic {
      width: 125px;
      margin: 12.5px 0 12.5px 0;
    }
    .univer-img-box .univer-pic:nth-child(7) {
      margin: auto;
    }

  .stud-case-p {
    margin-top: 12.5px;
  }

  .horizontal-line {
    margin-top: 25px;
    width: 75px;
  }

  .student-p {
    margin: 0 12.5px 0 25px;
    max-width: 95px;
  }

  .student-project .img-wrap:last-child {
    width: 100%;
  }
}

@media (max-width: 350px) {
  .univer-img-box .univer-pic {
    width: 100px;
  }
}

</style>
