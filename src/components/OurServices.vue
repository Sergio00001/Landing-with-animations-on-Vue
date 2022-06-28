<template>
    <div class="background">
        <div class="container">
            <div class="services__title" data-aos="slide-right" data-aos-duration="700">
                <h1 class="title">Our Services</h1>
            </div>
            <div class="services__text" data-aos="slide-left" data-aos-duration="700">
                <my-text class="text">skills and tools that enable businesses to take a step</my-text>
            </div>
            <Service :title="redesign" />
            <Service :title="smallBusiness" />
            <Service :title="eCommerse" />
        </div>
    </div>
</template>
<script>
import Service from '@/components/Service'
export default {
    components: { Service },

    data() {
        return {
            redesign: 'REDESIGN',
            smallBusiness: 'SMALL BUSINESS',
            eCommerse: 'E-Commerce'
        }
    }
}
</script>
<style scoped>
.background {
    position: relative;
    top: -10px;
    background-color: #1F2124;
}

.container {
    width: 90%;
    margin: 0 auto;
}

.title {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 700;
    font-size: 58px;
    line-height: 110%;
    letter-spacing: -2px;
    text-transform: uppercase;
    color: #F9CDCD;
    padding-top: 11vh;
    padding-bottom: 7vh;
}

.services__text {
    display: flex;
    justify-content: right;
}

.text {
    font-weight: 700;
    font-size: 32px;
    line-height: 110%;
    letter-spacing: -2px;
    text-transform: uppercase;
    color: #F2F4F3;
    max-width: 450px;
}

@media (max-width: 500px) {
    .title {
        font-size: 40px;
    }

    .services__text {
        justify-content: left;
    }

    .text {
        font-size: 5vw;
        letter-spacing: 0px;
    }
}
</style>