<template>
  <div class="contact-wrap l-spacing-sm">
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
            <div v-if="sendSuccess === false" class="form-header-c-ctx">
              <h6>info@youngtalent.cn</h6>
              <h6>400-961-1108</h6>
            </div>
          </div>
        </div>
        <div v-if="sendSuccess === false" class="form-inputs">
          <input class="inputName" :class="{'in-valid': validName === false}" type="text" name="name" placeholder="姓名" required>
          <input class="inputNumber" :class="{'in-valid': validNumber === false}" type="number" name="number" placeholder="电话" required>
          <input class="inputWechat" :class="{'in-valid': validWechat === false}" type="text" name="wechat" placeholder="微信号" required>
          <input class="inputEmail" :class="{'in-valid': validEmail === false}" type="email" name="email" placeholder="邮箱" required>
          <input class="inputMsg" :class="{'in-valid': validMsg === false}" type="text" name="msg" placeholder="信息" required>
          <p class="p-text">
            * 专业老师会尽快与你取得联系。您也可以通过网站上提供的地址、
            电话或邮箱直接联系我们
          </p>
        </div>
        <div v-if="sendSuccess === false" class="form-btns">
          <button @click="sendMessage" class="send-btn" type="button">提交信息</button>
          <button @click="closeForm" class="close-btn" type="button">关闭窗口</button>
        </div>
        <div v-if="sendSuccess === true" class="form-msg">
          <p class="p-text">
            您的预约申请已提交成功。<br>
            我们的专业老师会尽快与您取得联系。<br>
            谢谢！
          </p>
          <p class="p-text">
            Your message has been sent.<br>
            Our team will get back to you as soon as possible. Thank you!
          </p>
        </div>
        <div v-if="sendSuccess === true" class="logo-box">
          <div class="yellow-line"></div>
          <div class="yg-img">
            <img src="./assets/contactform/young_talent_logo_black.png" alt="">
          </div>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactUsForm',
  data () {
    return {
      sendSuccess: false,
      validNumber: null,
      validEmail: null,
      validName: null,
      validWechat: null,
      validMsg: null,
      contactFormValid: false
    }
  },
  methods: {
    closeForm () {
      this.$emit('close_form')
    },
    checkRegexValidation () {
      const checkEmail = /^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$/g
      const checkNumber = /^\+?-?\d+$/g
      const formNumber = document.querySelector('.inputNumber').value
      const formEmail = document.querySelector('.inputEmail').value
      const isValidNumber = formNumber.match(checkNumber)
      const isValidEmail = formEmail.match(checkEmail);

      (isValidNumber) ? this.validNumber = true : this.validNumber = false;
      (isValidEmail) ? this.validEmail = true : this.validEmail = false
    },
    checkOtherValidation () {
      (document.querySelector('.inputName').value !== '') ? this.validName = true : this.validName = false;
      (document.querySelector('.inputWechat').value !== '') ? this.validWechat = true : this.validWechat = false;
      (document.querySelector('.inputMsg').value !== '') ? this.validMsg = true : this.validMsg = false
    },
    sendMessage () {
      this.checkRegexValidation()
      this.checkOtherValidation();
      (this.validName === true && this.validNumber === true && this.validWechat === true && this.validEmail === true && this.validMsg === true) ? this.contactFormValid = true : this.contactFormValid = false

      if (this.contactFormValid === true) {
        this.sendSuccess = true
        setTimeout(() => {
          this.closeForm()
        }, 5000)
      }
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
        line-height: 1.7rem;
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
        border: 1px solid #ebe6e6;
      }
      .form-inputs > input:nth-child(5) {
        padding-bottom: 25px;
        height: 50px;
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

    .form-msg {
      text-align: left;
      margin-bottom: 100px;
    }

    .logo-box {
      display: flex;
      flex-direction: row;
      align-items: flex-end;
      justify-content: space-between;
    }
      .yg-img > img {
        display: block;
        width: 100px;
      }

/* Lines */
.purple-line {
  width: 50px;
  height: 5px;
  background-color: #b046aa;
  align-self: flex-end;
}
.yellow-line {
  max-width: 200px;
  width: 100%;
  height: 5px;
  background-color: #fccd0f;
  margin-right: 25px;
}
.form-inputs > .in-valid {
  border-color: red;
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
  .form-msg {
    text-align: left;
    margin-bottom: 50px;
  }
}
</style>
