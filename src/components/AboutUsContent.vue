<template>
    <div class="content">
        <div class="content__img" data-aos="fade-right" data-aos-duration="1000">
            <img class="img" :src="require('@/assets/images/aboutus/' + pic)" alt="picture">
        </div>
        <div class="content__discription">
            <div class="content__title" data-aos="zoom-in" data-aos-delay="50" data-aos-duration="1000">
                <h1 class="title">
                    {{ title }}
                </h1>
            </div>
            <div class="content__text">
                <div class="content__task" data-aos="zoom-in" data-aos-delay="150" data-aos-duration="1000">
                    <span class="text">TASK:</span><span class="text task">Conducted a review of the current site,
                        identified pain points that did not
                        allow
                        the client to be more recognizable to be more recognizable </span>
                </div>
                <div class="content__decision" data-aos="zoom-in" data-aos-delay="250" data-aos-duration="1000">
                    <span class="text">DECISION:</span><span class="text decision">Conducted a review of the current
                        site,
                        identified pain points that did not
                        allow
                        the client to be more recognizable to be more recognizable </span>
                </div>
            </div>
            <div class="content__controls" data-aos="zoom-in" data-aos-delay="350" data-aos-duration="1000">
                <my-text class="hash">#LANDING PAGE</my-text>
                <div class="details__btn">
                    <button class="btn">DETAILS</button>
                </div>
            </div>
        </div>
    </div>
    <hr>
</template>
<script>
export default {
    props: {
        pic: {
            type: String,
            default: ''
        },

        title: {
            type: String,
            default: ''
        }
    }
}
</script>
<style scoped>
.content {
    display: flex;
    align-items: center;
}

.content__discription {
    margin-left: 60px;
}

.content__img {
    padding: 30px 0px;
}

.img {
    max-width: 35vw;
}

.title {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 600;
    font-size: 34px;
    line-height: 49px;
    text-transform: uppercase;
    color: #1F2124;
    padding-bottom: 5vh;
}

.content__task {
    display: flex;
    justify-content: space-between;
}

.content__decision {
    display: flex;
    justify-content: space-between;
}

.text {
    font-family: 'Aileron';
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 28px;
    color: #1F2124;
    max-width: 500px;
    margin-bottom: 1vh;
}

.decision {
    margin-left: 60px;
}

.task {
    margin-left: 90px;
}

.content__controls {
    display: flex;
    justify-content: space-between;
    margin-top: 8vh;
    margin-bottom: 1vh;
}

.btn {
    font-family: 'Aileron';
    border: 1px solid #000000;
    border-radius: 30px;
    padding: 3px 10px;
    background-color: #ffffff00;
    color: #000000;
    letter-spacing: 0.03em;
    text-transform: uppercase;
    cursor: pointer;
    transition: all 0.5s ease 0s;
    font-size: 14px;
    line-height: 17px;
}

.btn:hover {
    color: rgb(255, 255, 255);
    background-color: #000000;
    padding: 5px 15px;
}


@media (max-width: 1024px) {

    .title {
        font-size: 20px;
    }

    .task {
        margin-left: 81px;
    }

    .text {
        font-size: 10px;
        line-height: 20px;
    }
}

@media (max-width: 768px) {
    .content {
        flex-direction: column;
    }

    .img {
        max-width: 100%;
    }

    .content__task {
        flex-direction: column;
    }

    .content__decision {
        flex-direction: column;
    }

    .task {
        margin-left: 0px;
    }

    .decision {
        margin-left: 0px;
    }

    .title {
        font-size: 28px;
    }

    .content__discription {
        margin-left: 0px;
    }

    .text {
        font-size: 13px;
    }

    .btn {
        width: 150px;
    }
}
</style>