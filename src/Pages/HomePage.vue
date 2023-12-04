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
      <div class="discounted-products">
        <div class="products-title">Товары со скидкой</div>
        <div class="products">
          <div class="item">
            <ProductComponent :imageId=1 :title="'Наполнитель комкующийся \'Pi-pi-Bent\' ,10л'" />
          </div>
          <div class="item">
            <ProductComponent :imageId=2 :title="'Сухой корм для крупных пород Pedigree, 13кг'" />
          </div>
          <div class="item">
            <ProductComponent :imageId=3 :title="'Наполнитель древесный \'Сибирская кошка\' , 7л'" />
          </div>
          <div class="item">
            <ProductComponent :imageId=4 :title="'Корм для щенков Acana Puppy, 340г'" />
          </div>
        </div>
        <div class="all_discount">все товары со скидкой</div>
      </div>
    </div>
  </div>
</template>

<script>
import ProductComponent from '../components/Product.vue';
export default {
  name: 'HomePage',
  components: {
    ProductComponent
  }
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

.discounted-products {
  margin-top: 330px;
}

.products-title {
  color: #99492E;
  font-size: 48px;
}

.products {
  margin-top: 68px;
  display: flex;
  justify-content: space-between;
}

.all_discount {
  width: 317px;
  height: 58px;
  border-radius: 16px;
  border: 2px solid #EC7C26;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #EC7C26;
  font-size: 24px;
  margin: 0 auto;
  margin-top: 55px;
}

.all_discount:hover {
  color: #FFE5D9;
  background-color: #CF6736;
}
</style>
