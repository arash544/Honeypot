<template>
  <div class="main-wrapper">
    <h2>"I like Honeypot because companies offer interviews with my base salary and above. It saved the effort of applying for jobs, doing interviews, getting offers, and finally finding out that the salary didn't meet my requirements."</h2>
    <div class="description-txt">
      <img src="Developer.jpg" alt />
      <div class="txt">
        <h5>Shuhei Kagawa</h5>
        <p>Hired as a Frontend Developer by Zalando</p>
      </div>
    </div>
    <Sidebg />
  </div>
</template>

<script>
import Sidebg from "./Sidebg";
export default {
  name: "Description",
  components: {
    Sidebg
  }
};
</script>

<style lang="scss" scoped>
.main-wrapper {
  display: flex;
  width: 100%;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
h2 {
  padding: 150px;
  text-align: center;
  font-weight: 400;
  @media only screen and (max-width: 768px) {
    padding: 20px 10px;
  }
}
img {
  width: 3vw;
  height: 3vw;
  border-radius: 100%;
  margin-right: 20px;
  @media only screen and (max-width: 768px) {
    width: 8vw;
    height: 9vw;
  }
}
.txt {
  display: flex;
  flex-direction: column;
}
.description-txt {
  display: flex;
  margin-top: 30px;
  color: gray;
  line-height: 1.1;
  padding: 10px;
}
</style>