<template>
  <div class="illustrate-wrap">
    <div class="img">
      <img src="illustration.png" alt />
    </div>
    <Textillustration />
  </div>
</template>

<script>
import Textillustration from "./Textillustration";
export default {
  name: "Imageillustration",
  components: {
    Textillustration
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
    width: 100vw;
  }
}
</style>