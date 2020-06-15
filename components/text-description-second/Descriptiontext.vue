<template>
  <div class="main-wrapper">
    <h2>"Honeypot was fantastic! I was surprised by the sheer amount of interview offers and the diversity of companies. My Talent Success Advisor gave me solid advice on how to structure a professional-looking CV, which is something I've always struggled with in the past."</h2>
    <div class="description-txt">
      <img src="developer1.jpg" alt />
      <div class="txt">
        <h5>Peter Ringelmann</h5>
        <p>
          Hired as a Frontend Developer by
          <br />Deutsche Post E-Post Development
        </p>
      </div>
    </div>
    <LeftSidebg />
    <RightSidebg />
  </div>
</template>

<script>
import LeftSidebg from "./LeftSidebg";
import RightSidebg from "./RightSidebg";
export default {
  name: "Descriptiontext",
  components: {
    LeftSidebg,
    RightSidebg
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
  margin-top: 150px;
  @media only screen and (max-width: 768px) {
    margin-top: 100px;
  }
}
h2 {
  padding: 20px 550px;
  text-align: center;
  font-weight: 400;
  @media only screen and (max-width: 768px) {
    padding: 0px 40px;
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
  line-height: 1.2;
  padding: 10px;
}
</style>