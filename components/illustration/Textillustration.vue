<template>
  <div class="wrap">
    <h1>
      Join an Engineering
      <br />Team in Your Ideal Role
    </h1>
    <p>On Honeypot, over 1000 companies are hiring Software Developers, DevOps Engineers and Engineering Leaders just like you!</p>
    <a href="/">Signup to Honeypot</a>
  </div>
</template>

<script>
export default {
  name: "Textillustration"
};
</script>

<style lang="scss" scoped>

.wrap {
  display: flex;
  width: 45%;
  flex-direction: column;
  padding-top: 50px;
  padding-left: 20px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    padding-left: 0;
    padding-top: 10px;
    text-align: center;
  }
  @media only screen and (max-width: 768px) {
    padding: 10px 30px;
  }
}
p {
  color: gray;
  margin-top: 0px;
  font-weight: 450;
  @media only screen and (max-width: 768px) {
    padding: 10px 30px;
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