<template>
  <div class="main-wrap">
    <div class="wrap">
      <h1>
        Choose the Locations
        <br />that Suit You
      </h1>
      <p>Honeypot operates in Europe’s most exciting tech cities. Set your location preference and companies apply to you!</p>
      <a href="/">Signup to Honeypot</a>
    </div>
    <Locationimage />
  </div>
</template>

<script>
import Locationimage from "./Locationimage";
export default {
  name: "Locationtext",
  components: {
    Locationimage
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
  width: 45%;
  padding-left: 300px;
  flex-direction: column;
  padding-bottom: 100px;
  justify-content: center;
  align-items: right;

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
  justify-content: right;
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