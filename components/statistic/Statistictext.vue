<template>
  <div class="main-wrap">
    <div class="wrap">
      <h1>Know Your Worth!</h1>
      <p>Companies apply directly to you so you can compare offers side by side. No more job applications or clumsy back and forths with headhunters.</p>
      <a href="/">Signup to Honeypot</a>
    </div>
    <Statisticimage />
  </div>
</template>

<script>
import Statisticimage from "./Statisticimage";
export default {
  name: "Statistictext",
  components: {
    Statisticimage
  }
};
</script>

<style lang="scss" scoped>
.main-wrap {
  display: flex;
  flex-direction: row;
  width: 100%;
  margin-top: 150px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    flex-direction: column;
    margin-top: 30px;
  }
}
.wrap {
  display: flex;
  width: 50%;
  flex-direction: column;
  padding: 50px 50px 100px 550px;

  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    padding-left: 0;
    padding-top: 30px;
    text-align: center;
  }
  @media only screen and (max-width: 420px) {
  }
}
p {
  color: gray;
  margin-top: 0px;
  font-weight: 450;
  @media only screen and (max-width: 768px) {
    padding: 10px 90px;
  }
}
a {
  font-weight: 600;
  @media only screen and (max-width: 768px) {
    padding-bottom: 10px;
  }
}
h1 {
  font-weight: 400;
}
a::after {
  content: url("data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTEiIGhlaWdodD0iOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMTAuNzggMy4zOTZMNy42OTMuMjVhLjg0My44NDMgMCAwIDAtMS4xOTUgMCAuODg0Ljg4NCAwIDAgMCAwIDEuMjE4bDEuNjM2IDEuNjdILjg0N0EuODYuODYgMCAwIDAgMCA0YS44Ni44NiAwIDAgMCAuODQ3Ljg2NGg3LjI5OUw2LjQ5OCA2LjUzM2EuODg0Ljg4NCAwIDAgMCAwIDEuMjE4QS44MzYuODM2IDAgMCAwIDcuMDkgOGMuMjIgMCAuNDI5LS4wODMuNTkxLS4yNDlsMy4wNzUtMy4xMzZBLjg1Ljg1IDAgMCAwIDExIDQuMDEyYzAtLjIyNS0uMDctLjQ2Mi0uMjItLjYxNnoiIGZpbGw9IiMzNjg1RDYiIGZpbGwtcnVsZT0ibm9uemVybyIvPjwvc3ZnPg==");
}
</style>