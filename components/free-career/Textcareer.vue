<template>
  <div class="wrap">
    <h1>
      Free Career Support
      <br />and Guidance
    </h1>
    <p>Your Talent Success Advisor will guide you through from start to finish, providing guidance on your resume and interviews, helping you benchmark your salary, evaluate offers and find a job you love.</p>
    <a href="/">Signup to Honeypot</a>
  </div>
</template>

<script>
export default {
  name: "Textcareer"
};
</script>

<style lang="scss" scoped>
.wrap {
  display: flex;
  width: 45%;
  flex-direction: column;
  padding-top: 100px;
  padding-left: 100px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
    padding-left: 0;
    margin-top: 20px;
    text-align: center;
  }
  @media only screen and (max-width: 768px) {
    padding: 10px 30px;
  }
}
p {
  padding-right: 400px;
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