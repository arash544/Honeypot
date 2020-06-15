<template>
  <div class="illustrate-wrap">
    <div class="img">
      <img src="one-bear.png" alt />
    </div>
    <Techtext />
  </div>
</template>

<script>
import Techtext from "./Techtext";
export default {
  name: "Techimage",
  components: {
    Techtext
  }
};
</script>

<style lang="scss" scoped>
.illustrate-wrap {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
  margin-top: 100px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    flex-direction: column;
    margin-top: 50px;
  }
}
.img {
  width: 45%;
  display: flex;
  justify-content: flex-end;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    padding-bottom: 10px;
  }
}
img {
  width: 26vw;
  @media only screen and (max-width: 768px) {
    width: 60vw;
  }
}
</style>