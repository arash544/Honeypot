<template>
  <div class="wraped">
    <img src="two-bears.png" alt />
  </div>
</template>

<script>
export default {
  name: "Signupimage"
};
</script>

<style lang="scss" scoped>
.wraped {
  width: 50%;
  flex-direction: row;
  padding-top: 50px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    text-align: center;
    order: -1;
  }
}
img {
  width: 30vw;
  padding-left: 50px;
  @media only screen and (max-width: 768px) {
    padding-bottom: 20px;
    width: 70vw;
  }
  @media only screen and (max-width: 420px) {
    width: 100%;
    padding-right: 100px;
  }
}
</style>