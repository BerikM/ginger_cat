<template>
    <div class="footer">
        <div class="container">
            <div class="sub-container about-us">
                <div class="title">О нас</div>
                <p>Мы гордимся нашей бригадой профессионалов, готовых помочь вам и вашим пушистым друзьям на каждом этапе.
                    Наша цель - обеспечить ваших питомцев всем необходимым для счастливой и здоровой жизни, предоставляя
                    широкий выбор качественных товаров и экспертные консультации. Вместе мы делаем мир животных ярче и
                    комфортнее!</p>
            </div>
            <div class="sub-container information">
                <div class="information-item title">Информация</div>
                <div class="information-item">Контакты</div>
                <div class="information-item">Найти друга</div>
                <div class="information-item">Профиль</div>
            </div>
            <div class="sub-container contacts-data">
                <div class="contacts-item"><img src="../assets/footer/phone.svg" alt="" srcset=""> +7 702 854 35 18</div>
                <div class="contacts-item"><img src="../assets/footer/map-tag.svg" alt="" srcset=""> Улица Камзина, 171 102а
                    бутик; 1 этаж</div>
                <div class="contacts-item"><img src="../assets/footer/mail.svg" alt="" srcset=""> ryzhiy_kot_pvl@gmail.com
                </div>
            </div>
            <div class="social">
                <div class="whatsapp"><img src="../assets/footer/whatsapp.svg" alt="" srcset=""> </div>
                <div class="instagramm"><img src="../assets/footer/instagram.svg" alt="" srcset=""> </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'FooterComponent'
}
</script>

<style scoped>
.footer {
    background-color: #FFE5D9;
    width: 100%;
    height: 378px;
    font-family: 'Mulish', sans-serif;
}

.container {
    width: 1181px;
    height: 280px;
    margin: 0 auto;
    padding-top: 62px;
    display: grid;
    grid-template-columns: 1.5fr 1fr 1fr;
    color: #DD926E;
}

.sub-container {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

p {
    max-width: 381px;
    font-size: 15;
    line-height: 19px;
}

.title {
    font-size: 32px;
    font-weight: 700;
    color: #99492E;
}

.about-us {
    height: 207px;
}

.information {
    height: 207px;
    font-size: 24px;
}

.contacts-data {
    width: 359px;
    height: 236px;
    font-size: 24px;
    word-wrap: break-word;
}

.contacts-item {
    display: flex;
    align-items: center;
}

img {
    margin-right: 21px;
}

.social {
    display: flex;
}

.instagramm {
    margin-left: 75px;
}
</style>