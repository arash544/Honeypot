<template>
  <div class="wrapper">
    <h1>Top Jobs for Top Tech Talent</h1>
    <p>Be part of the top 10% and connect with Europe’s top tech companies.</p>
  </div>
</template>

<script>
export default {
  name: "Topjobtext"
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 150px;
  line-height: 2.6;
  text-align: center;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    align-items: center;
    margin-top: 0px;
    text-align: center;
    line-height: unset;
  }
  @media only screen and (max-width: 420px) {
    width: 100%;
    justify-content: center;
    align-items: center;
    text-align: center;
    line-height: unset;
  }
}
p {
  color: gray;
  @media only screen and (max-width: 768px) {
    padding-right: 10px;
    padding-left: 10px;
  }
}
h1 {
  font-weight: 400;
}
</style>