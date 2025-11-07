<script setup>
import { ref } from 'vue'

const activeIndex = ref(0)

const menuItems = [
    'Главная',
    'Каталог',
    'Бренды',
    'Доставка и оплата',
    'Помощь',
    'Компания'
]

const setActive = (index) => {
    activeIndex.value = index
}
</script>

<template>
    <div class="header__row">
        <div class="header__item">
            <a href="#">
                <img src="/assets/logo.svg" alt="Logo" class="header__logo">
            </a>
        </div>
        <div class="header__item">
            <nav>
                <ul>
                    <li
                        v-for="(item, index) in menuItems"
                        :key="index"
                        :class="{'nav__first-child': activeIndex === index}"
                        @click="setActive(index)"
                    >
                        <a href="#">{{ item }}</a>
                    </li>
                </ul>
            </nav>
        </div>
        <div class="header__item">
            <a href="#">
                <img src="/assets/search.svg" alt="Search" class="header__icon">
            </a>
            <a href="#">
                <img src="/assets/like.svg" alt="Like" class="header__icon">
            </a>
            <a href="#">
                <img src="/assets/shop.svg" alt="Shop" class="header__icon">
            </a>
        </div>
    </div>
</template>

<style>
body {
    max-width: 1920px;
    padding-inline: 20px;
    font-family: 'Poppins', sans-serif;
}

.header__row {
    padding: 20px 0;
}

.header__row,
nav ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}

.header__logo {
    max-width: 100%;
    width: 230px;
}

nav ul {
    background-color: #E9EDF3;
    padding: 12px 20px 12px 20px;
    border-radius: 50px;
    gap: 25px;
}

.nav__first-child {
    background-color: #17BE79;
    border-radius: 50px;
    padding: 10px 25px;
}

.nav__first-child a {
    font-size: 16px;
    color: #fff;
}

nav ul li a {
    font-size: 16px;
    color: #272B37;
}

nav ul li {
    cursor: pointer;
}

.header__item:last-child {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    gap: 10px;
}

.header__item:last-child a {
    background-color: #17BE79;
    border-radius: 50%;
    padding: 12px;
}

.header__icon {
    max-width: 100%;
    width: 16px;
}
</style>
