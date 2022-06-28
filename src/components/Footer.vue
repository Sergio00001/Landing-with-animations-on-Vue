<template>
    <div class="container">
        <div class="footer__top">
            <div class="footer__logo" data-aos="fade-right" data-aos-duration="1000">
                <img src="@/assets/images/footer/footer_logo.png" alt="logo">
            </div>
            <div class="footer__title" data-aos="fade-left" data-aos-delay="50" data-aos-duration="1000">
                <h1 class="top__title">We collaborate with ambitious brands and people. Let's build. </h1>
            </div>
        </div>
        <div class="footer__bottom">
            <div class="footer__form" data-aos="fade-up" data-aos-duration="1000">
                <form action="#">
                    <h5 class="bottom__title">Stay in the Know</h5>
                    <input type="email" class="form__email" placeholder="Email Address"><img
                        class="arrow animate__animated animate__slow"
                        :class="{ 'animate__hinge': this.animate === true }" src="@/assets/images/footer/arrow.png"
                        alt="arrow">
                </form>
            </div>
            <div class="footer__links">
                <div class="footer__social" data-aos="fade-left" data-aos-delay="150" data-aos-duration="1000">
                    <h5 class="bottom__title">Social</h5>
                    <a href="#"
                        class="social__link animate__animated animate__pulse animate__infinite animate__slow">Instagram</a>
                    <a href="#"
                        class="social__link animate__animated animate__pulse animate__infinite animate__slow">Facebook</a>
                    <a href="#"
                        class="social__link animate__animated animate__pulse animate__infinite animate__slow">Telegram</a>
                </div>
                <div class="footer__site" data-aos="fade-left" data-aos-delay="350" data-aos-duration="1000">
                    <h5 class="bottom__title">Site</h5>
                    <a href="#"
                        class="social__link animate__animated animate__pulse animate__infinite animate__slow animate__delay-1s">Works</a>
                    <a href="#"
                        class="social__link animate__animated animate__pulse animate__infinite animate__slow animate__delay-1s">Our
                        Services</a>
                </div>
            </div>
        </div>
    </div>
    <div class="form__copyright">
        <h5 class="copy">Modern Site ©</h5>
    </div>
</template>
<script>
export default {
    data() {
        return {
            animate: false
        }
    },

    methods: {
        startAnimation() {
            setInterval(() => {
                if (this.animate === false) {
                    this.animate = true
                    setTimeout(() => {
                        this.animate = false
                    }, 2000);
                } else {
                    this.animate = false
                }
            }, 10000);
        }
    },

    mounted() {
        this.startAnimation()
    },
}
</script>
<style scoped>
.container {
    width: 90%;
    margin: 0 auto;
}

.footer__top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 90px;
    margin-bottom: 50px;
}

.top__title {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 700;
    font-size: 32px;
    line-height: 110%;
    letter-spacing: -1px;
    text-transform: uppercase;
    color: #1F2124;
    max-width: 500px;
}

.footer__bottom {
    display: flex;
    justify-content: space-between;
}

.footer__links {
    display: flex;
    margin-bottom: 100px;
}

.bottom__title {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 700;
    font-size: 16px;
    line-height: 30px;
    text-transform: uppercase;
    color: #1F2124;
}

.footer__form {
    position: relative;
}

.form__email {
    height: 40px;
    width: 400px;
    border-top: 0px solid;
    border-left: 0px solid;
    border-right: 0px solid;
    border-bottom: 1px solid #1F2124;
    padding-left: 10px;
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 400;

}

.form__email::placeholder {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 29px;
    color: #1f212481;
}

input {
    outline: none;
}

.arrow {
    position: absolute;
    right: 0px;
    height: 18px;
    transition: all 0.3s ease 0s;
}

.arrow:hover {
    height: 23px;
}

.footer__social {
    display: flex;
    flex-direction: column;
    margin-right: 189px;
}

.footer__site {
    display: flex;
    flex-direction: column;
    margin-right: 150px;
}

.social__link {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 35px;
    color: #1F2124;
    border-bottom: 0px solid;
    transition: all 0.3s ease 0s;
}

.form__copyright {
    background-color: #E7E7E7;
}

.copy {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 600;
    font-size: 11px;
    line-height: 49px;
    text-align: center;
    text-transform: uppercase;
    color: #5E5E5E;
}


@media(max-width: 1120px) {
    .top__title {
        max-width: 350px;
        font-size: 21px;
    }

    .form__email {
        width: 300px;
    }

    .footer__site {
        margin-right: 0px;
    }
}

@media(max-width: 767px) {
    .footer__top {
        flex-direction: column;
        align-items: start;
    }

    .footer__logo {
        margin-bottom: 40px;
    }

    .footer__bottom {
        flex-direction: column;
    }

    .footer__form {
        margin-bottom: 40px;
        inline-size: fit-content;
    }
}

@media(max-width:400px) {
    .footer__social {
        margin-right: 0px;
    }

    .footer__links {
        justify-content: space-around;
    }

    .form__email {
        width: 280px;
    }
}
</style>