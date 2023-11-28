<template>
    <div class="header">
        <img src="../assets/header/logo.svg" alt="">
        <div class="menu">
            <a href="#" class="menu-item">Каталог</a>
            <a href="#" class="menu-item">Профиль</a>
            <a href="#" class="menu-item">Найти друга</a>
            <a href="#" class="menu-item">Полезная информация</a>
        </div>
        <div class="search">
            <form>
                <input type="text" placeholder="Поиск..">
                <button type="submit"><img src="../assets/header/search.svg" alt="" srcset=""></button>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderComponent',

}
</script>


<style scoped>
.header {
    margin: 0 auto;
    width: 1180px;
    height: 102px;
    font-family: 'Mulish', sans-serif;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.menu {
    width: 587px;
    display: flex;
    justify-content: space-between;
}

.menu-item {
    color: #cf6736;
    font-size: 20px;
    text-decoration: none;
}

.search input {
    width: 279px;
    height: 40px;
    padding-left: 24px;
    background-color: #FFE5D9;
    border: none;
    border-radius: 24px;
    color: #DD926E;
}

.search input:focus {
    outline: none;
}

.search button {
    width: 20px;
    height: 20px;
    background: none;
    border: none;
    position: relative;
    top: 5px;
    left: -48px;
}
</style>