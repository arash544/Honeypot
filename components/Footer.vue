<template>
  <div class="txt-wrapper">
    <div class="first-col">
      <img class="logo" src="bear.svg" alt />
      <p>© 2020 Honeypot</p>
      <ul>
        <li>
          <a href="/">EN</a>
        </li>
        <li>
          <a href="/">DE</a>
        </li>
        <li>
          <a href="/">NL</a>
        </li>
      </ul>
    </div>
    <div class="second-col">
      <b>
        <a href="/">FOR TALENTS</a>
      </b>
    </div>
    <div class="third-col">
      <div class="cover">
        <b>
          <a href="/">FOR EMPLOYERS</a>
        </b>
        <a href="/">Pricing</a>
      </div>
    </div>

    <div class="fourth-col">
      <div class="cover">
        <b>
          <a href="/">ABOUT US</a>
        </b>
        <a href="/">Press</a>
        <div class="career">
          <a href="/">Careers</a>
          <img
            class="logo"
            src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAAAYCAYAAACRD1FmAAAAAXNSR0IArs4c6QAABgVJREFUaAXtWltsVEUY/ubs/VrabZeWQmmx5VJFkGtrTDDB+uKLt3hBY/SBRAP6gA+ooCD4QIwaExM1+mDUAIEHoy8awBjjQ0tpC2rEQgu2tFjYbi/u7uned8d/ZsOy7bJntxcvkJ3knJ35b2fmm///5z+7y5CncX7WDjXwDsAfAeflecSLbIEAwzDdjsJu2MnYuqA+Lyqq/2MC96m8ckWB6whwuMkpt0ONmYm4lV3nZPc47zVBHQkQyIZsbpGSFwHGgrA3ObU9OeQtB0cR4Lxo5hDg3Aq0lSg52EXyHCJQBHkOwcxlqghyLmTmkJ4HZEXzYJyrefBkZK5M/S/t5ASZqydbkODHtGbd17YTo31fp0VUbxe6TzyeHovOue+fRmD41CTa1EHvT9vhG/pxKrngsffiUQz3fHlD+YGu/Yiql7N4seBVXOrYk0WfDuHciS1QvZ15VbJA5uHO27i/7Rskk8epdGvUsuCsbIbfcx3AAPXj4XFEg1ekWjwyRv0h2MtXa5lBafVm6E1lmjIzZZbXPQyDlcrWKU1vdqFiyaNTqNMbMp0JTDHmVUqXcPLNbsK3C7HYDiqk82uSaef8Jgyd/Yh6SboUBEa64G54EgFPO1x1D5IHdxLAa+REErEALv/8LsL+Pih6i5QrWbBJTtDsrIXNdSfi0XEMdh2AZV4DYsFhLFr7GoJjv+Pyr+/RC5QCvcGJhatfhtFaJfUyb1GS72/fjZD/IsyOOtRt3E86OgxfOILqlduoa5xku2rlC/D0HERd8wGMXfoOkYlBRAKXEPL9Qc+vR+2GN+WaohNDGOh6C9GwF9Z5y2Awl9O6m+GYvxEKAawQ0PmawjlnXG19Bqqvh7B6hby3IICFYYO1EgaTC6Hx8xBeq+jMKKm+l7y7XT43QKHkrGyS/cEzb8NaugLLNn+G+nvep/A+BJ5I5WIHbZZsyQQClHJsZXdIgBNRP/o796BmzatYuukTVDVuxdBvH6Zkp9wj6gBqaFNWtByC2FB15LSUiAU94Mk4+cFk22IcDXmkTCIeoM08S/q7seL+Q4iFR0n/F8nznP+CAG1CY8thucGq9zSphiRP0ZsKAxnqyX0E7uf00pHtHtKU9k2mDG8HeW0HHO710ovEgglBSRO7Dh6H/2objLYq+jxJQJ6GyVFNm9GaZdxkXyQXJRhik4zmCko5HtJrlYsPB/rTm5Op7HCvowih2p++OLC5VpJnplJWpkym7Uy66Kf0LdRjsJN+VP1TrsFP54m7/jEi66E3lpLtVWlVmS4K8WTmaH4dOgPFNA7TlUhbKLAjPDXg6SRA2yXIQk147NjAMdplIwFbTZ6UoACJUzrwkcePy8tevpbCfoHmU3giSkdDLK0jdN31T5AnpSIglzKjhcyukT5jNO8YRYWf+robmrPOWw6d3nZDXiZRHnzMtv4Mc9y9BXpWT8Y/IKsTmUJafZtrNeXBHkyMdRO4y6Wow70BV7o/lblLEMSO20pvh8IMKFv8gLyErIVynFazV9yFKHmkiBahV7rwPvKyVdAZnVpqc8ZjlP7M9sXkMN9KmzwRRvCvc2n75UseornY0+NcnfTBJwSYpbmfPl7ivHUvVGUbJbIXKY1UCF6uxhSDPLQUJlJ5qlgRoRfr8MiD8Zpezdpd6O94A96+r5CMBSFCt3bDPjrPcn81YrDMpzy4A+d/eA6WkgY6lC6gcvmzcNkXXjP7j3+KPN9/ag+8vUdozjXy4COk5HMvUOkp5mevWKc5D8244qG2WsR4n6aFaTITER/lTrP07sJVOZWGo9CbRZmX2sjCdWcnKV6UmEIVBKU7kTa6j28h59grozDN03qEA65Jnpwly3ksizZLgs5UMgMLjAD+b34vEGVeRB2EtWQpAqNnKKKWyBJTLEKCX8BqtD052FqNOLJflwowfCuJhHy9VLd7YC1rnP5LU15PvpWQmsVaxHkgrpm2fzfBzXSWN7meNsiWihEq6eY8L9/kmBU+ffHzE5p9miAz1iCq/qOFWy1KTkHgIGMsoV1dCA2783n6S4BKNUzxLwFTEMw5zPhLgJD5G80aIdSz4HlpAAAAAElFTkSuQmCC"
            alt
          />
        </div>

        <a href="/">FAQ</a>
        <a href="/">Legal Notice</a>
        <a href="/">Privacy Policy</a>
        <a href="/">Cookie declaration</a>
        <a href="/">Terms of Service</a>
      </div>
    </div>
    <div class="fifth-col">
      <div class="cover">
        <b>
          <a href="/">COMMUNITY</a>
        </b>
        <a href="/">Blog</a>
        <a href="/">GraphQL Conf</a>
      </div>
    </div>

    <div class="sixth-col">
      <div class="cover">
        <b>
          <a href="/">WE'RE SOCIAL, TOO!</a>
        </b>
        <div class="career">
          <img src="twitter.png" />
          <a href="/">Twitter</a>
        </div>
        <div class="career">
          <img src="facebook.png" />
          <a href="/">Facebook</a>
        </div>
        <div class="career">
          <img src="linkedin.png" />
          <a href="/">Linkedin</a>
        </div>
        <div class="career">
          <img src="github.png" />
          <a href="/">Github</a>
        </div>
        <div class="career">
          <img src="instagram.png" />
          <a href="/">Instagram</a>
        </div>
        <div class="career">
          <img src="youtube.png" />
          <a href="/">Youtube</a>
        </div>
        <div class="career">
          <img src="mail.svg" />
          <a href="/">hello@honeypot.io</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style lang="scss" scoped>
.cover {
  display: flex;
  flex-direction: column;
  @media only screen and (max-width: 768px) {
  }
}
.txt-wrapper {
  display: flex;
  flex-wrap: wrap;
  margin-top: 50px;
  flex-direction: row;
  width: 100%;
  justify-content: center;
}
.third-col,
.fourth-col {
  @media only screen and (max-width: 768px) {
    padding-left: 30px;
  }
}
.sixth-col {
  @media only screen and (max-width: 768px) {
    padding-left: 80px;
  }
}
.first-col,
.second-col,
.third-col,
.fourth-col,
.fifth-col,
.sixth-col {
  display: flex;
  align-items: center;
  flex-direction: column;
  padding-top: 50px;
  height: 400px;
  width: 16%;
  @media only screen and (max-width: 768px) {
    width: 100%;
    height: auto;
    margin-top: 10px;
    padding-top: 10px;
    padding-bottom: 10px;
  }
}
li {
  list-style-type: none;
}
a {
  color: gray;
  margin: 5px;
  @media only screen and (max-width: 768px) {
    font-size: 20px;
  }
}
ul {
  display: flex;
  flex-direction: row;
  padding-right: 50px;
  @media only screen and (max-width: 768px) {
    padding: auto;
  }
}
p {
  color: gray;
}
.career {
  margin: 5px;
}
img {
  @media only screen and (max-width: 768px) {
    width: 4vw;
  }
}
.logo {
  @media only screen and (max-width: 768px) {
    width: 14vw;
  }
}
</style>