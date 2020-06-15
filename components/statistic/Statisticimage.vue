<template>
  <div class="img">
    <img src="statistic.svg" alt />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.img {
  width: 40%;
  display: flex;
  margin-left: 50px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-left: 0;
    justify-content: center;
    order: -1;
  }
}
</style>