<template>
    <div class="background">
        <div class="container">
            <div class="hidden__nav">
                <div class="nav__logo" data-aos="fade-in" data-aos-duration="1000">
                    <img src="@/assets/images/footer/footer_logo.png" alt="logo">
                </div>
                <div class="nav__btn" data-aos="fade-in" data-aos-duration="1000">
                    <img src="@/assets/images/footer/hidden_nav_btn.png" alt="btn">
                </div>
            </div>
            <div class="about__title" data-aos="fade-right" data-aos-duration="1000">
                <h1 class="title">Our work will
                    tell about us</h1>
            </div>
            <div class="about__nav">
                <div class="about__links" data-aos="zoom-in" data-aos-duration="1000">
                    <a href="#" class="about__link">ALL CASE</a>
                    <a href="#" class="about__link">e-commerce</a>
                    <a href="#" class="about__link">LANDING</a>
                    <a href="#" class="about__link">corporate</a>
                </div>
                <div class="about__text" data-aos="fade-left" data-aos-duration="1000">
                    <my-text class="text">The work we create lives at the intersection of clarity and surprise and
                        positions
                        brands
                    </my-text>
                </div>
            </div>
            <hr>
            <AboutUsContent :pic="pictureTop" :title="titleTop" />
            <AboutUsContent :pic="pictureCenter" :title="titleCenter" />
            <AboutUsContent :pic="pictureBottom" :title="titleBottom" />
        </div>
    </div>
</template>
<script>
import AboutUsContent from '@/components/AboutUsContent'
export default {
    components: { AboutUsContent },

    data() {
        return {
            pictureTop: 'Image_1.png',
            titleTop: 'TELEVISION MANAGER SERVICES',
            pictureCenter: 'Image_2.png',
            titleCenter: 'E-COMMERCE video productions',
            pictureBottom: 'Image_3.png',
            titleBottom: 'E-COMMERCE DIGITAL AGENCY'
        }
    }
}
</script>
<style scoped>
.background {
    background: #E5E5E5;
    position: relative;
    top: -7px;
    padding-bottom: 70px;
}

.container {
    width: 90%;
    margin: 0 auto;
}

.title {
    padding-top: 11vh;
    padding-bottom: 7vh;
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 700;
    max-width: 485px;
    font-size: 58px;
    line-height: 110%;
    letter-spacing: -2px;
    text-transform: uppercase;
    color: #1F2124;
}

.about__nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.about__link {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 400;
    font-size: 1.5vh;
    line-height: 47px;
    color: #1F2124;
    margin-right: 20px;
    text-transform: uppercase;
    border-bottom: 0px solid;
    transition: all 0.3s ease 0s;
}

.about__link:hover {
    font-size: 2.5vh;
    border-bottom: 1px solid #1F2124;
}

.text {
    font-size: 16px;
    line-height: 29px;
    color: #1F2124;
    max-width: 319px;
    margin-bottom: 30px;
}

.hidden__nav {
    padding-top: 25px;
    display: none;
}

@media (max-width: 767px) {
    .about__text {
        display: none;
    }

    .hidden__nav {
        display: flex;
        justify-content: space-between;
    }
}

@media (max-width: 390px) {
    .title {
        font-size: 50px;
    }

    .about__link {
        font-size: 1.5vh;
    }
}
</style>