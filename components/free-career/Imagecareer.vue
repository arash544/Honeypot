<template>
  <div class="illustrate-wrap">
    <div class="img">
      <img src="woman1.png" alt />
    </div>
    <Textcareer />
  </div>
</template>

<script>
import Textcareer from "./Textcareer";
export default {
  name: "Imagecareer",
  components: {
    Textcareer
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
    margin-top: 30px;
  }
}
.img {
  width: 50%;
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
    width: 70vw;
  }
}
</style>