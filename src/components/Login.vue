<template>
  <div id="login">
    <div class="modal-mask">
      <div class="modal-wrapper">
        <div class="modal-container">
          <div class="main"></div>
          <div class="form">
            <h3>Sign up</h3>
            <div v-show="true" class="register">
              <input type="text" placeholder="username" />
              <input type="password" placeholder="password" />
              <div class="button">Create an account</div>
            </div>
            <h3>Sign in</h3>
            <div v-show="false" class="login">
              <input type="text" placeholder="username" />
              <input type="password" placeholder="password" />
              <div class="button">Sign in</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less">
.modal-mask {
  position: fixed;
  z-index: 100;
  background-color: rgba(0, 0, 0, 0.65);
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: table;
  transition: opacity 0.3s ease;
}

// 这里 modal-wrapper 的作用是为了使登录 UI 在垂直方向居中，是一种传统的 css 方法
// 其实这里用 flex 实现的话 页面就不用多加上这个 modal-wrapper div 了
// 只需要在 modal-mask（父级div）里使用 display：flex
// 然后加上 justify-content：center 和 align-items：center 就可以搞定
.modal-wrapper {
  border: 1px solid red;
  display: table-cell;
  vertical-align: middle;
}

.modal-container {
  border: 1px solid purple;
  width: 800px;
  height: 500px;
  margin: 0px auto;
  background-color: #fff;
  border-radius: 4px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.33);
  transition: all 0.3s ease;
  font-family: Arial, Helvetica, sans-serif;
  display: flex;

  .main {
    flex: 1;
    background: #36bc64 url();
    background-size: contain;
  }

  .form {
    width: 270px;
    border-left: 1px solid #ccc;

    h3 {
      padding: 10px 20px;
      font-weight: normal;
      font-size: 16px;
      border-top: 1px solid #eee;
      cursor: pointer;

      &:nth-of-type(2) {
        border-bottom: 1px solid #eee;
      }
    }

    .button {
      background-color: #2bb964;
      height: 36px;
      line-height: 36px;
      text-align: center;
      font-weight: bold;
      color: #fff;
      border-radius: 8px;
      margin-top: 18px;
      cursor: pointer;
    }

    .login,
    .register {
      padding: 10px 20px;
      border-top: 1px solid #eee;

      input {
        display: block;
        width: 100%;
        height: 35px;
        line-height: 35px;
        padding: 0 6px;
        border-radius: 4px;
        border: 1px solid #ccc;
        outline: none;
        font-size: 14px;
        margin-top: 10px;
      }

      input:focus {
        border: 3px solid #9dcaf8;
      }

      p {
        font-size: 12px;
        margin-top: 10px;
        color: #444;
      }

      .error {
        color: red;
      }
    }

    .login {
      border-top: 0;
    }
  }
}
</style>
