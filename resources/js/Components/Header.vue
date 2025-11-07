<script setup>

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
                    <li class="nav__first-child">
                        <a href="#">Главная</a>
                    </li>
                    <li>
                        <a href="#">Каталог</a>
                    </li>
                    <li>
                        <a href="#">Бренды</a>
                    </li>
                    <li>
                        <a href="#">Доставка и оплата</a>
                    </li>
                    <li>
                        <a href="#">Помощь</a>
                    </li>
                    <li>
                        <a href="#">Компания</a>
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
    width: 100%;
}

nav ul {
    background-color: #E9EDF3;
    padding: 16px 30px 16px 16px;
    border-radius: 50px;
    gap: 30px;
}

.nav__first-child {
    background-color: #17BE79;
    border-radius: 50px;
    padding: 10px 25px;
}

.nav__first-child a {
    font-size: 18px;
    color: #fff;
}

nav ul li a {
    font-size: 18px;
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
    padding: 14px;
}
</style>
