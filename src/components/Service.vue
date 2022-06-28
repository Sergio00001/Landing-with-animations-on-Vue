<template>
    <hr class="hr">
    <div class="service">
        <div class="service__title" data-aos="fade-right" data-aos-duration="1000">
            <h1 class="title">{{ title }}</h1>
        </div>
        <div class="service__wrapper">
            <div class="service__info">
                <div class="info__header" data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                    <h1 class="header">REDESIGN WEB-SITE</h1>
                </div>
                <div class="info__text" data-aos="fade-up" data-aos-delay="50" data-aos-duration="1000">
                    <my-text class="text">Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be
                        more recognizable Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be more recognizable </my-text>
                </div>
                <div class="info__header" data-aos="fade-up" data-aos-delay="150" data-aos-duration="1000">
                    <h1 class="header">REDESIGN WEB-SITE</h1>
                </div>
                <div class="info__text" data-aos="fade-up" data-aos-delay="150" data-aos-duration="1000">
                    <my-text class="text">Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be
                        more recognizable Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be more recognizable </my-text>
                </div>
            </div>
            <div class="service__info">
                <div class="info__header" data-aos="fade-up" data-aos-delay="250" data-aos-duration="1000">
                    <h1 class="header">REDESIGN WEB-SITE</h1>
                </div>
                <div class="info__text" data-aos="fade-up" data-aos-delay="250" data-aos-duration="1000">
                    <my-text class="text">Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be
                        more recognizable Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be more recognizable </my-text>
                </div>
                <div class="info__header" data-aos="fade-up" data-aos-delay="350" data-aos-duration="1000">
                    <h1 class="header">REDESIGN WEB-SITE</h1>
                </div>
                <div class="info__text" data-aos="fade-up" data-aos-delay="350" data-aos-duration="1000">
                    <my-text class="text">Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be
                        more recognizable Conducted a review of the current site, identified pain points that did
                        not
                        allow
                        the
                        client to be more recognizable </my-text>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        title: {
            type: String,
            default: ''
        }
    }
}
</script>
<style scoped>
.hr {
    border: 1px solid #F9CDCD;
    margin: 30px 0px;
}

.service {
    display: flex;
    justify-content: space-between;
}

.title {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 700;
    font-size: 34px;
    line-height: 110%;
    letter-spacing: -2px;
    text-transform: uppercase;
    color: #F9CDCD;
}

.service__wrapper {
    display: flex;
    margin-top: 2vh;
    margin-bottom: 3vh;
    margin-right: 1.5vh;
}

.service__info {
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
}

.service__info:first-child {
    margin-right: 8vw;
}

.header {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 600;
    font-size: 22px;
    line-height: 110%;
    text-transform: uppercase;
    color: #F9CDCD;
    margin-top: 2vh;
}

.text {
    max-width: 300px;
    font-size: 16px;
    line-height: 29px;
    color: #FEFCFF;
    margin-top: 2vh;
}

@media(max-width: 1120px) {

    .header {
        font-size: 17px;
    }

    .title {
        font-size: 20px;
    }

    .text {
        font-size: 14px;
        line-height: 20px;
    }
}

@media(max-width: 950px) {
    .service {
        flex-direction: column;
    }

    .service__info:last-child {
        display: none;
    }

    .title {
        letter-spacing: 0px;
    }

    .text {
        max-width: 100%;
    }
}
</style>