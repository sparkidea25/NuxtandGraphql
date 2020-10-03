<template>
  <div class="container">
    <div class="box a">
      <div class="innerfirst">
        <p>Slideshows</p>
    </div>
    <span class="icon is left">
    <font-awesome-icon :icon="['fas', 'envelope']" />
    </span>
    </div>
    <div class="box b" style="width: 3px">
      <div class="rectup"></div>
      <div class="formbox">
        <form class="">
          <h1>Create Free account</h1>
          <label for="email">Email:</label><br /><br />
          <input type="text"  id="email"/>
          <br />
          <br />
          <label for="password">Password:</label><br /><br />
          <input type="text" id="password" />
          <br />
          <br />
          <label for="Create username">Create Username:</label><br /><br />
          <input type="text" id="create-username">
          <br />
          <br />
          <VuePhoneNumberInput v-model="myValue" />
          <p>Get referral code</p>
          <button>Signup</button>
        </form>

        <p>Have an account? Signin to explore</p>
        <br /><br /><br /><br />
        <div class="col">

          </div>
      </div>
      <div class="rectdown"></div>
    </div>
  </div>
</template>

<script>
import VuePhoneNumberInput from 'vue-phone-number-input';
export default {

}
</script>

<style>
  .container {
    width: 100%;
    height: 100vh;
    display: flex;
    -webkit-flex-wrap: nowrap;
    flex-wrap: nowrap;
  }

  .box {
    height: 100vh;
    min-width: 20vh;
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    background-size: auto;
    background-position: center;
    background-repeat: no-repeat;
  }

  .innerfirst {
    position: absolute;
    padding: 30px;
    height: 400px;
    width: 250px;
    background-color: #B395FF;
    border-radius: 60px;

  }

.rectdown {
  top: 500px;
  left: 1200px;
  width: 150px;
  height: 200px;
  background-color: #B395FF40;
  border-radius: 32px;
  position: absolute;
}

.rectup {
  bottom: 500px;
  right: 500px;
  width: 150px;
  height: 200px;
  background-color: #B395FF40;
  border-radius: 32px;
  position: absolute;
}

.formbox {
  width: 400px;
  height: 600px;
  background-color: white;
  position: absolute;
  border-radius: 50px;

}

  .a {
    background-color: #4F388A;
  }

  .b {
    background-color: #2E1963;
    width: 30px;
  }

  h1 {
    font-family: Basis Grotesque Pro;
  }
  form {
    padding: 40px;
  }

  input[type=text] {
    width: 250px;
    height: 20px;
    border: none;
    border-bottom: 2px solid black;
  }

  button {
    background-image: linear-gradient(#432B7B, #6A4BBC);
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
  }
</style>
