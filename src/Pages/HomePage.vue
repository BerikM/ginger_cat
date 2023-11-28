<template>
  <div class="home_page">
    <div class="background-cat">
      <img src="../assets//background//cat.png" alt="" srcset="">
    </div>
    <div class="container">
      <div class="main">
        <div class="main-title">
          Заботьтесь о своих питомцах с нами!
        </div>
        <div class="main-text">Наш зоомагазин - это место, где встречаются забота и радость. Широкий выбор товаров
          высокого качества и заботливый уход для ваших домашних любимцев. Приходите к нам, чтобы сделать жизнь ваших
          пушистых и пернатых друзей еще счастливее!</div>
        <div class="button-contact">Связаться с нами</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
}
</script>

<style scoped>
.background-cat {
  position: absolute;
  top: 10px;
  right: -50px;
  transform: rotate(8.82deg);
  z-index: -1;
}

.container {
  width: 1183px;
  margin: 0 auto;
  margin-top: 164px;
  font-family: 'Mulish', sans-serif;
}

.main-title {
  font-family: 'Sofia Sans Semi Condensed', sans-serif;
  width: 780px;
  height: 182px;
  font-size: 84px;
  font-weight: 900;
  line-height: 85px;
  color: #CF6736;
}

.main-text {
  width: 680px;
  word-wrap: break-word;
  font-size: 24px;
  color: #EC7C26;
}

.button-contact {
  width: 472px;
  height: 119px;
  margin-top: 95px;
  border: 3px solid #CF6736;
  border-radius: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #CF6736;
  font-size: 40px;
}

.button-contact:hover {
  background-color: #CF6736;
  color: #FFE5D9;
}
</style>
