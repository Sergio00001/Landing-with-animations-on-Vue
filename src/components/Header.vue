<template>
  <div class="header">
    <div class="header__background">
      <img class="background__img" src="@/assets/images/header/header_background.jpg" alt="background">
      <div class="container">
        <img src="@/assets/images/header/header_logo.png" alt="logo" class="header__logo" data-aos="fade-in"
          data-aos-delay="850" data-aos-duration="1000">
        <img src="@/assets/images/header/navbar_btn.png" alt="btn" class="navbar__btn" data-aos="fade-left"
          data-aos-delay="650" data-aos-duration="1000">
        <div class="header__content">
          <h1 class="header__title" data-aos="fade-in" data-aos-delay="450" data-aos-duration="1000">Purpose-driven
            experiences convert customer
            attention and loyalty</h1>
          <my-text class="header__text" data-aos="fade-in" data-aos-delay="250" data-aos-duration="1000">Modernsite
            designs and develops
            beautifully designed and cutting-edge e-commerce
            and
            small business
            websites around customer needs.</my-text>
          <div class="header__control">
            <my-button class="header__btn" data-aos="fade-in" data-aos-duration="1000">Start
              Growing</my-button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
.container {
  width: 90%;
}


.header__background {
  position: relative;
}

.background__img {
  width: 100%;
  height: auto;
}

.header__logo {
  position: absolute;
  top: 20px;
  left: 44%;
}

.navbar__btn {
  position: absolute;
  top: 2%;
  left: 90%;
  cursor: pointer;
  transition: all 0.3s ease 0s;
  height: 1vh;
}

.navbar__btn:hover {
  height: 2vh;
}

.header__content {
  position: absolute;
  top: 23%;
}

.header__title {
  font-family: 'Poppins';
  font-size: 5vw;
  line-height: 120%;
  text-align: center;
  letter-spacing: -2px;
  color: #F9CDCD;
  padding-bottom: 3%;
}

.header__text {
  text-align: center;
  color: #FCFCFC;
  max-width: 68vw;
  margin: 0 auto;
  font-size: 2.5vh;
  line-height: 125%;
}

.header__control {
  display: flex;
  justify-content: center;
  margin-top: 5%;
}

.header__btn {
  font-size: 2vh;
  line-height: 120%;
}

@media(max-width:767px) {
  .header {
    display: none;
  }
}
</style>
