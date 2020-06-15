<template>
  <div class="wrapper">
    <div class="main-txt">
      <div class="signup-head">
        <h1>
          A Simple and Quick Sign
          <br />Up Process!
        </h1>
      </div>
      <div class="text-wrap">
        <div class="btn-wrap-first">
          <button class="btn-signup">01</button>
        </div>
        <div class="text first-txt">
          <h4>Create a Profile</h4>
          <p>
            It’s your chance to tell us what you want in your
            <br />next role - and it takes less than 5 minutes.
          </p>
        </div>
      </div>
      <div class="text-wrap">
        <div class="btn-wrap">
          <button class="btn-signup">02</button>
        </div>
        <div class="text second-txt">
          <h4>Complete our Screening</h4>
          <p>
            Pass our code screening and take an optional call
            <br />with your Talent Success Advisor, who positions you
            <br />to receive the best offers.
          </p>
        </div>
      </div>
      <div class="text-wrap">
        <div class="btn-wrap">
          <button class="btn-signup">03</button>
        </div>
        <div class="text third-txt">
          <h4>Become Visible and Get Offers</h4>
          <p>
            Become visible on Honeypot so that companies can
            <br />find your profile and make you offers with salary
            <br />and tech stack up front.
          </p>
        </div>
      </div>
      <div class="text-wrap">
        <div class="btn-wrap-fourth">
          <button class="btn-signup">04</button>
        </div>
        <div class="text fourth-txt">
          <h4>Get Hired</h4>
          <p>
            Interview with companies that interest you! And
            <br />choose the one you like the best.
          </p>
        </div>
      </div>
    </div>
    <Signupimage />
  </div>
</template>

<script>
import Signupimage from "./Signupimage";
export default {
  components: {
    Signupimage
  }
};
</script>

<style lang="scss" scoped>
.main-txt {
  display: flex;
  flex-direction: column;
  width: 44%;
  @media only screen and (max-width: 768px) {
    width: 100%;
    display: flex;
    justify-content: center;
  }
}
.wrapper {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
  margin-top: 100px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    flex-direction: column;
    margin-top: 50px;
    justify-content: center;
  }
}
.signup-head {
  display: flex;
  justify-content: flex-end;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    text-align: center;
    padding-top: 20px;
  }
}
h1 {
  padding-right: 20px;
  font-weight: 400;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    padding-right: 0;
  }
}
p {
  color: gray;
  line-height: 1.3;
}
.text-wrap {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  padding-right: 15px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    padding-top: 20px;
  }
}
.first-txt {
  padding-right: 25px;
}
.fourth-txt {
  padding-right: 25px;
}
.btn-signup {
  color: #cea000;
  border: 1px solid #fff2c6;
  background-color: #fff2c6;
}
.btn-wrap {
  margin-right: 35px;
  padding-top: 20px;
}
.btn-wrap-first {
  margin-right: 35px;
  padding-top: 20px;
}
.btn-wrap-fourth {
  margin-right: 38px;
  padding-top: 20px;
}
h4 {
  font-size: 19px;
}
</style>