<template>
  <div class="txt-wrapper">
    <div class="first-column">
      <img src="photo1.jpg" alt />
      <h5>Emil Ahlbäck</h5>
      <p>Hired as a Senior Frontend Developer by Weissmaler</p>
      <h6>"After only two weeks I received 13 interview invites from a great selection of companies. From these I could choose the ones that best suited me and ended up finding the perfect startup job."</h6>
    </div>
    <div class="second-column">
      <img src="photo2.jpg" alt />
      <h5>Veronica Hannibal</h5>
      <p>Hired as a JavaScript Developer by finAPI</p>
      <h6>"Within a few weeks I received multiple job offers and landed an awesome job right after finishing my degree. Compared to my experience with job recruiters on other platforms, my experience on Honeypot felt much more personal."</h6>
    </div>
    <div class="third-column">
      <img src="photo3.jpg" alt />
      <h5>Sashen Singh</h5>
      <p>Hired as a Mobile Engineer by Aperto</p>
      <h6>"The user experience was amazing, the site was really easy to use. The platform does all the heavy lifting for you, you don't need to search or keep track of where you apply. Their system is really efficient in the sense that companies find you, making this a really simple and painless platform to use."</h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "Employee"
};
</script>

<style lang="scss" scoped>
.txt-wrapper {
  display: flex;
  margin-top: 50px;
  justify-content: center;
  align-items: center;
  padding: 20px 190px;
  @media only screen and (max-width: 768px) {
    padding: 0;
    width: 100%;
    flex-direction: column;
  }
}
img {
  width: 4vw;
  border-radius: 100%;
  @media only screen and (max-width: 768px) {
    width: 15vw;
  }
}
p {
  color: gray;
}
h5 {
  margin-top: 10px;
}
.first-column,
.second-column,
.third-column {
  text-align: center;
  flex-direction: row;
  padding: 50px 60px;
  height: auto;
  width: 25%;
  align-self: stretch;
  @media only screen and (max-width: 768px) {
    padding: 20px 40px;
    width: 100%;
  }
}
</style>