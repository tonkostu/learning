<template>
  <div class="hello">
    <div class="logo">
      <h1>facebook</h1>
    </div>
    <div class="login-box shadow rounded">
      <h2>{{ msg }}</h2>   
      <div class="Input">
        <div class="input-mail">
          <input class="form-control" type="text" placeholder="メールアドレスまたは電話番号:" >
        </div>
        <div class="input-password mt-3">
          <input class="form-control" type="password" placeholder="パスワード">
        </div>
      </div> 
      <div class="Button-login">
        <button type="button" class="btn btn-primary mt-3">
          ログイン
        </button>
      </div>
      <div class="forget mt-3">
        <a href="" class="">アカウントを忘れた場合</a>
      </div>
      <div class="or-box mt-2">
        <span class="mataha">
          または
        </span>
      </div>
      <div class="button-create">
        <button type="button" class="btn btn-success">
          新しいアカウントを作成
        </button>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'loginppage',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
  color: blue;
  
}
h2{
 padding: 24px 0 16px 0;
  font-size: 20px;
  height: 70px;
}
a {
  text-decoration: none;
  color: rgb(0, 102, 255);
}
span{
      display: inline-block;
    position: relative;
}
.form-control{
  margin-left: auto;
  margin-right: auto;
  width: 300px;
}
.login-box{
  box-shadow: 5px;
  margin: auto;
  width: 380px;
  padding: 0 0 14px 0;
}
.btn{
  width: 300px;
}
.or-box{
    display: block;
    margin-bottom: 10px;
    margin-top: 10px;
    overflow: hidden;
    text-align: center;
    white-space: nowrap;
    margin-left: 8px;
    margin-right: 8px;
    width: auto;
}
.or-box>span:after, .or-box>span::before{
 
    background: #ccd0d5;
    content: "";
    height: 1px;
    position: absolute;
    top: 50%;
    width: 9999px;


}
.or-box>span::before{
    margin-right: 15px;
    right: 100%
}
.or-box>span::after{
    left: 100%;
    margin-left: 15px;
}
</style>
