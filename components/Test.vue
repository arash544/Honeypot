<template>
  <div class="wrapper">
    <div class="main-text">
      <h1>
        A Simple and Quick Sign
        <br />Up Process!
      </h1>
      <div class="button-signup">
        <button class="btn-signup">01</button>
      </div>
      <div class="txt">
        <h4 class="first-title">Create a Profile</h4>
        <p>
          It’s your chance to tell us what you want in your
          <br />next role - and it takes less than 5 minutes.
        </p>
      </div>
      <div class="button-signup">
        <button class="btn-signup">02</button>
      </div>
      <div class="txt">
        <h4 class="second-title">Complete our Screening</h4>
        <p>
          Pass our code screening and take an optional call
          <br />with your Talent Success Advisor, who positions you
          <br />to receive the best offers.
        </p>
      </div>
      <div class="button-signup">
        <button class="btn-signup">03</button>
      </div>
      <div class="txt">
        <h4 class="third-title">Become Visible and Get Offers</h4>
        <p>
          Become visible on Honeypot so that companies can
          <br />find your profile and make you offers with salary
          <br />and tech stack up front.
        </p>
      </div>
      <div class="button-signup">
        <button class="btn-signup">04</button>
      </div>
      <div class="txt">
        <h4 class="fourth-title">Get Hired</h4>
        <p>
          Interview with companies that interest you! And
          <br />choose the one you like the best.
        </p>
      </div>
    </div>
    <div class="wraped">
      <img src="two-bears.png" alt />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.wraped {
  //   display: flex;
  width: 45%;
  //   flex-direction: row;
  //   padding-top: 50px;
  //   margin-left: -200px;
  //   border: 1px solid blue;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    margin-left: 0;
    // padding-left: 0;
    // padding-top: 10px;
    // text-align: center;
  }
}
.wrapper {
  display: flex;
  width: 100%;
  flex-direction: row;
  border: 1px solid blue;
  margin-top: 50px;
}
.main-text {
  display: flex;
  width: 45%;
  flex-direction: column;
  border: 1px solid blue;
}
h1 {
  justify-content: flex-end;
  display: flex;
  border: 1px solid blue;
  font-weight: 400;
}
.txt {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-top: -45px;
  // align-self: center;
  // justify-content:flex-end;
  // border: 1px solid blue;
}
p,
h4 {
  // justify-content:flex-end;
  align-self: flex-end;
  border: 1px solid blue;
}
p {
  color: gray;
}
h4 {
  margin-right: 178px;
//   align-self: left;
  font-size: 19px;
}
.first-title{
    margin-right: 213px;
}
.second-title{
    margin-right: 150px;
}
.third-title{
    margin-right: 178px;
}
.fourth-title{
    margin-right: 178px;
}
.button-signup {
  justify-content: center;
  display: flex;
  margin-top: 20px;
}
.btn-signup {
  color: #cea000;
  border: 1px solid #fff2c6;
  background-color: #fff2c6;
}
</style>