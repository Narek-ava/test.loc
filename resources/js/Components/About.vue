<script setup>
</script>

<template>
    <div class="about">
        <h2>Товары, которые покупают чаще всего</h2>

        <div class="about__row">
            <div class="about__item">
                <div class="about-block">
                    <div class="about__item-box">
                        <img src="/assets/block.svg" alt="Image">
                        <p>Аппаратные<br>кошельки</p>
                    </div>
                    <a href="#" class="send">
                        <img src="/assets/Arrow%202%20(Stroke).svg" alt="Image">
                    </a>
                </div>
                <div class="about-block">
                    <div class="about__item-box">
                        <img src="/assets/block.svg" alt="Image">
                        <p>U2F-токены</p>
                    </div>
                    <a href="#" class="send">
                        <img src="/assets/Arrow%202%20(Stroke).svg" alt="Image">
                    </a>
                </div>
            </div>
            <div class="about__item">
                <div class="about__sec-block">
                    <div class="about__item-box">
                        <img src="/assets/block.svg" alt="Image">
                        <p>Устройства для записи seed</p>
                    </div>
                    <p class="about__item-box-desc">Надежные устройства для хранения мнемонической фразы,<br> необходимой для восстановления доступа к вашим средствам</p>
                    <a href="#" class="send">
                        <img src="/assets/Arrow%202%20(Stroke).svg" alt="Image">
                    </a>
                </div>
                <div class="about-bg">
                    <h3>Популярные категории</h3>
                </div>
                <div class="about__sec-block">
                    <div class="about__item-box">
                        <img src="/assets/block.svg" alt="Image">
                        <p>Устройства для записи seed</p>
                    </div>
                    <p class="about__item-box-desc">Надежные устройства для хранения мнемонической фразы,<br> необходимой для восстановления доступа к вашим средствам</p>
                    <a href="#" class="send">
                        <img src="/assets/Arrow%202%20(Stroke).svg" alt="Image">
                    </a>
                </div>
            </div>
            <div class="about__item">
                <div class="about-block">
                    <div class="about__item-box">
                        <img src="/assets/block.svg" alt="Image">
                        <p>Аксессуары</p>
                    </div>
                    <a href="#" class="send">
                        <img src="/assets/Arrow%202%20(Stroke).svg" alt="Image">
                    </a>
                </div>
                <div class="about-block">
                    <div class="about__item-box">
                        <img src="/assets/block.svg" alt="Image">
                        <p>Чехлы и кейсы</p>
                    </div>
                    <a href="#" class="send">
                        <img src="/assets/Arrow%202%20(Stroke).svg" alt="Image">
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.about {
    padding: 60px 20px;
}
h2 {
    font-size: 51px;
    color: #272B37;
}
.about__row {
    margin-top: 60px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}
.about__item:nth-child(1) {
    width: 24.5%;
}
.about__item:nth-child(2) {
    width: 50%;
}
.about__item:nth-child(3) {
    width: 24.5%;
}
.about-block {
    width: 100%;
    height: 60vh;
    background-color: #E9EDF3;
    padding: 30px;
    margin-top: 10px;
    position: relative;
    border-radius: 20px;
}
.about__item-box {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 20px;
    margin-bottom: 80px;
}
.about__item-box img {
    background-color: #fff;
    border-radius: 50%;
    padding: 12px 15px;
}
.about__item-box p {
    font-size: 30px;
    color: #272B37;
    line-height: 26px;
}
.about__sec-block {
    background-color: #E9EDF3;
    padding: 30px;
    margin-top: 10px;
    position: relative;
    border-radius: 20px;
}
.about__item-box-desc {
    font-size: 18px;
    color: #272B37;
    line-height: 20px;
    margin: 16px 0 0 75px;
}
.about-bg {
    background-image: url(/assets/Rectangle 2340 1.png);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    border-radius: 30px;
    padding: 211px 0;
    display: flex;
    justify-content: center;
    margin-top: 10px;
}
h3 {
    position: relative;
    font-size: 51px;
    padding: 50px;
    color: #fff;
    border-radius: 30px;
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(38.31px);
    -webkit-backdrop-filter: blur(38.31px);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

</style>
