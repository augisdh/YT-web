<template>
  <div class="contact-wrap">
    <div class="contact-form-box margin-sides">
      <form class="form" novalidate>
        <div class="form-header">
          <div class="form-header-i-box">
            <h4>
              个人信息
              <span>PERSONAL INFORMATION</span>
            </h4>
          </div>
          <div class="form-header-c-box">
            <div class="purple-line"></div>
            <div class="form-header-c-ctx">
              <h6>info@youngtalent.cn</h6>
              <h6>400-961-1108</h6>
            </div>
          </div>
        </div>
        <div class="form-inputs">
          <input type="text" name="name" placeholder="姓名" required>
          <input type="number" name="number" placeholder="电话" required>
          <input type="?" name="?" placeholder="微信号" required>
          <input type="email" name="email" placeholder="邮箱" required>
          <input type="text" name="msg" placeholder="信息" required>
          <p class="p-text">
            * 专业老师会尽快与你取得联系。您也可以通过网站上提供的地址、
            电话或邮箱直接联系我们
          </p>
        </div>
        <div class="form-btns">
          <button class="send-btn" type="button">提交信息</button>
          <button @click="closeForm" class="close-btn" type="button">关闭窗口</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactUsForm',
  methods: {
    closeForm () {
      this.$emit('close_form')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.contact-wrap {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-color: rgba(0, 0, 0, .4);
  z-index: 20;
  display: flex;
  justify-content: center;
  align-items: center;
}

.contact-form-box {
  max-width: 500px;
  width: 100%;
  background-color: #fafafa;
}
  .form {
    margin: 50px;
    display: flex;
    flex-direction: column;
  }
    .form-header {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      margin-bottom: 50px;
    }

    .form-header-i-box {
      text-align: left;
    }
      .form-header-i-box > h4 {
        margin: 0;
        font-size: 2rem;
      }
        .form-header-i-box > h4 span {
          display: block;
          font-size: 1rem;
        }
    .form-header-c-box {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      text-align: right;
    }
      .form-header-c-ctx > h6 {
        margin: 0;
        font-size: .8rem;
        color: #b046aa;
      }

    .form-inputs {
      display: flex;
      flex-direction: column;
      margin-bottom: 50px;
    }
      .form-inputs > input {
        height: 25px;
        margin-bottom: 25px;
        padding-left: 10px;
      }
      .form-inputs > input:nth-child(5) {
        padding-bottom: 25px;
      }
      .form-inputs .p-text {
        text-align: left;
        font-size: .8rem;
        margin: 0;
      }

    .form-btns {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    }
      .form-btns > button {
        max-width: 150px;
        width: 100%;
        font-size: 16px;
        font-weight: 700;
        padding: 5px 0;
        border: none;
        cursor: pointer;
        color: #fff;
      }
      .send-btn {
        background-color: #fccd0f;
        margin-right: 10px;
      }
      .close-btn {
        background-color: #ebe6e6;
        margin-left: 10px;
      }

/* Lines */
.purple-line {
  width: 50px;
  height: 5px;
  background-color: #b046aa;
  align-self: flex-end;
}

/* @Media */
@media (max-width: 550px) {
  .form {
    margin: 25px;
  }
  .form-header,
  .form-inputs {
    margin-bottom: 25px;
  }
}
</style>
