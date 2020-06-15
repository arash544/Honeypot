<template>
  <div class="img">
    <img src="three-bears.png" alt />
  </div>
</template>

<script>
export default {
  name: "Locationimage"
};
</script>

<style lang="scss" scoped>
.img {
  width: 45%;
  display: flex;
  justify-content: flex-start;

  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    order: -1;
  }
}
img {
  width: 30vw;
  padding-left: 40px;
  padding-top: 30px;
  @media only screen and (max-width: 768px) {
    width: 60vw;
    padding-top: 30px;
    padding-left: 0;
  }
}
</style>