<template>
  <q-page class="flex flex-center" style="background: #f5f7f5;">
    <!-- title -->
    <div class="full-width top-img header gt-xs">
      <div class="title text-left text-h3 text-bold title-top q-pt-xl q-pl-xl">
        <q-img src="/logo.svg" style="width: 15vmax; height: auto" />
      </div>
      <div class="title text-center text-h4 text-bold title-bottom full-width q-pa-md">
        <span class="full-width">
          Правильная упаковка для правильных продуктов
        </span>
      </div>
    </div>

    <div class="full-width top-img header lt-sm">
      <div class="title text-left text-h3 text-bold title-top q-pt-xl q-pl-xl">
        <q-img src="/logo.svg" style="width: 15vmax; height: auto" />
      </div>
      <div class="title text-center text-h5 text-bold title-bottom full-width q-pa-md">
        <span class="full-width">
          Правильная упаковка для правильных продуктов
        </span>
      </div>
    </div>

    <!-- products -->
    <div class="row text-h6 text-center full-width q-ma-lg gt-xs">
      <div class="fit row wrap justify-center content-center q-gutter-xl">
        <q-card class="my-card" v-for="group in groups" :key="group.img" @click="scrollToText(group.ref)">
          <q-img :src="group.img" :ratio="1" style="width:250px">
            <div class="absolute-bottom text-subtitle2 text-center">
              {{ group.title }}
            </div>
          </q-img>
        </q-card>
      </div>
    </div>

    <div class="row text-h6 text-center full-width q-my-lg lt-sm">
      <div class="fit row wrap justify-center content-center q-gutter-y-lg">
        <q-card class="my-card" v-for="group in groups" :key="group.img" @click="scrollToText(group.ref)">
          <q-img :src="group.img" :ratio="1" style="width:250px">
            <div class="absolute-bottom text-subtitle2 text-center">
              {{ group.title }}
            </div>
          </q-img>
        </q-card>
      </div>
    </div>

    <div class="row full-width q-py-md">
      <div class="col-xs-12 col-sm-12 col-md-4"></div>
      <div class="col-xs-12 col-sm-12 col-md-8 bg-indigo-9 text-left text-h3 text-bold text-white q-pa-md headlines">
        &nbsp;Продукция
      </div>
    </div>

    <div class="row q-pt-md">
      <div class="col-xs-12">
        <div class="text-h5 product" ref="description" id="description" label="UF">
          <span class="text-bold">Стаканы c УФ печатью</span> является наиболее распространенным и экономичным
          способом декорирования стаканов. Печать на стаканы производится ультрафиолетовыми красками, прочно
          закрепляющимися на поверхности стакана.
        </div>
      </div>
    </div>

    <div class="row q-pt-lg">
      <div class="col-xs-12">
        <div class="text-h5 product" ref="description1" id="description1">
          <span class="text-bold ">Стакан с картонной этикеткой – комбинация пластика и картона.</span> На наружную
          поверхность
          изготовленного полипропиленового стакана наклеивается картонная этикетка.
        </div>
      </div>
    </div>

    <div class="row q-pt-lg">
      <div class="col-xs-12">
        <div class="text-h5 product" ref="description2" id="description2">
          <span class="text-bold ">Стакан с термоусадочной этикеткой.</span> На наружную поверхность полипропиленового
          стакана усаживается термоусадочная этикетка. Печать наносится на внутреннюю поверхность этикетки, благодаря
          чему изображение долго сохраняет свою насыщенность и не истирается.
        </div>
      </div>
    </div>

    <div class="row q-pt-lg">
      <div class="col-xs-12">
        <div class="text-h5 product" ref="description3" id="description3">
          <span class="text-bold ">Крышки на стаканы.</span> Мы производим полипропиленовые крышки «нахлобучки»
          (поверх крышки для фольги) высокого качества, пригодные для надевания на стакан на высокоскоростных
          разливочных линиях.
        </div>
      </div>
    </div>

    <q-btn icon="shopping_cart" no-caps color="deep-orange" glossy class="text-h4 q-my-lg place-order"
      @click="scrollTo()">
      Оформить заказ
    </q-btn>

    <!-- quality & safety -->
    <div class="row full-width q-pt-md">
      <div class="col-xs-12 col-sm-12 col-md-8  bg-indigo-9 text-right text-h3 text-bold text-white q-pa-md headlines">
        Качество и безопасность
      </div>
      <div class="col-xs-12 col-sm-12 col-md-4 "></div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify safety">
          <q-img src="product/a4.jpg" class="q-ml-xl float-right" style="max-width:600px; height: auto;" />
          Все наше производство устроено так, как если бы мы производили детское питание - это позволяет нам
          гарантировать чистоту и безопасность нашей продукции. Начиная от полимерной гранулы и заканчивая готовой
          упаковкой с декором - мы отслеживаем качество упаковки всех стадиях производства. Это позволяет нам выпускать
          достойный продукт со стабильным качеством.
        </div>
      </div>
    </div>

    <div class="row q-pt-lg">
      <div class="col">
        <div class="text-h5 text-center text-indigo-9 text-bold slogan">
          ООО «MIDAS PLASTICS» — производство полного цикла
        </div>
      </div>
    </div>

    <div class="row q-pt-lg">
      <div class="col">
        <div class="text-h5 text-justify safety">
          Весь путь от гранулы до готовой упаковки с печатью полностью проходит на одной территории, что позволяет нам
          отслеживать весь процесс и производить качественный продукт.</div>
      </div>
    </div>

    <!-- tools -->
    <div class="row full-width q-pt-lg">
      <div class="col-xs-12 col-sm-12 col-md-4"></div>
      <div class="col-xs-12 col-sm-12 col-md-8 bg-indigo-9 text-left text-h3 text-bold text-white q-pa-md headlines">
        Наше производство
      </div>
    </div>

    <!-- description -->
    <!-- first card -->
    <div class="row full-width q-pt-lg flex-center">
      <div class="col-xs-12 col-sm-6">
        <q-img src="tools/1.png" class="list-photo q-ma-lg q-ml-xl" style="width: 80%;" />
      </div>
      <div class="col-xs-12 col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left list-text">
          <div class="col-1 text-right">
            ✔&nbsp;
          </div>
          <div class="col">
            оснащено лучшим в мире оборудованием европейского производства
          </div>
        </div>
        <div class="row q-px-lg q-pt-lg text-h5 text-left list-text">
          <div class="col-1 text-right">
            ✔&nbsp;
          </div>
          <div class="col">
            обеспечивает высокую производительность
          </div>
        </div>
      </div>
    </div>

    <!-- second card -->
    <div class="row full-width  flex-center">
      <div class="col-xs-12 col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left list-text">
          <div class="col-1 text-right">
            ✔&nbsp;
          </div>
          <div class="col">
            позволяет производить широкий ассортимент стаканов различных форм и объемов без <br />значительных
            инвестиций в дорогостоящие пресс-формы
          </div>
        </div>
      </div>

      <div class="col-xs-12 col-sm-6 flex-center gt-xs">
        <q-img src="product/a1.png" class="list-photo q-ma-lg" style="width: 80%;" />
      </div>
      <div class="col-xs-12 col-sm-6 flex-center lt-sm">
        <q-img src="product/a1.png" class="list-photo q-ma-lg float-right" style="width: 80%;" />
      </div>
    </div>


    <!-- placing orders -->
    <div class="row full-width q-pt-lg">
      <div class="col-xs-12 col-sm-12 col-md-4"></div>
      <div class="col-xs-12 col-sm-12 col-md-8 bg-indigo-9 text-left text-h3 text-bold text-white q-pa-md headlines"
        ref="ordering">
        &nbsp;Прием заказов
      </div>
    </div>

    <div class="row full-width q-pt-md">
      <div class="col-md-8 text-center">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3071.069332161991!2d66.93449035323566!3d39.67065494165193!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3f4d19f6d85e60d1%3A0xb4d60d21fc6f24ae!2z0J7QntCeICLQotCe0J3QkyI!5e0!3m2!1sru!2s!4v1673002782281!5m2!1sru!2s"
          width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" class="map"
          referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>

      <div class="col-md-4">
        <div class="q-pa-md">
          <div class="row">
            <div class="col-xs-1 col-sm-3 col-md-1 text-primary text-h6 icon"><span class="material-icons">phone&nbsp;
              </span></div>
            <div class="col-xs-11 col-sm-9 col-md-11 text-h6 contacts"><a href="tel:+998933338575"
                style="color: darkorchid;">
                +998 93 333-85-75
              </a> <br />
              <a href="tel:+998937203338" style="color: darkorchid;">
                +998 93 720-33-38
              </a>
            </div>
          </div>
        </div>
        <div class="q-pa-md">
          <div class="row">
            <div class="col-xs-1 col-sm-3 col-md-1 text-primary text-h6 icon"><span class="material-icons">place&nbsp;
              </span></div>
            <div class="col-xs-11 col-sm-9 col-md-11 text-h6 contacts">Узбекистан, г. Самарканд, ул. Гагарина, 36.
            </div>
          </div>
        </div>
        <div class="q-pa-md">
          <div class="row">
            <div class="col-xs-1 col-sm-3 col-md-1 text-primary text-h6 icon"><span class="material-icons">mail&nbsp;
              </span></div>
            <div class="col-xs-11 col-sm-9 col-md-11 text-h6 contacts"><a
                href="mailto:info@midasplastics.uz">info@midasplastics.uz</a>
            </div>
          </div>
        </div>
      </div>

    </div>
  </q-page>
</template>

<script setup>
import { defineComponent, ref } from "vue";
import { scroll } from 'quasar';
const { getScrollTarget, setVerticalScrollPosition } = scroll;

const groups = [
  { img: "product/a5.jpg", title: "Cтакан с УФ печатью", ref: "description" },
  { img: "product/a6.jpg", title: "Стакан с картонной этикеткой", ref: "description1" },
  { img: "product/a7.jpg", title: "Стакан с термоусадочной этикеткой", ref: "description2" },
  { img: "product/a8.jpg", title: "Крышки на стаканы", ref: "description3" },
]

const ordering = ref(null);
const scrollTo = () => {
  const el = ordering.value
  const target = getScrollTarget(el)
  const offset = el.offsetTop
  const duration = 300
  setVerticalScrollPosition(target, offset, duration)
}

const description = ref(null);
const description1 = ref(null);
const description2 = ref(null);
const description3 = ref(null);
let el;
let target;
let offset;
let duration;
const scrollToText = (data) => {
  if (data === description.value.id) {
    el = description.value;
  }
  else if (data === description1.value.id) {
    el = description1.value;
  }
  else if (data === description2.value.id) {
    el = description2.value;
  }
  else {
    el = description3.value;
  }
  target = getScrollTarget(el);
  offset = el.offsetTop;
  duration = 300;
  setVerticalScrollPosition(target, offset, duration);
}


</script>

<style lang="sass" scoped>
.top-img
  background: url(/tools/2.png)
  background-size: cover
  background-position: center
  background-attachment: fixed
  background-repeat: no-repeat

.header
  position: relative
  min-height: 550px

.title
  color: #f5f7f5
  text-shadow: 1px 1px #000000
.title-bottom
  position: absolute
  top: 250px
  background-image: linear-gradient(rgba(0,0,0,0), rgba(0,0,0,1))
  height: 300px
  display: flex

.title-top
  background-image: linear-gradient(rgba(0,0,0,1), rgba(0,0,0,0))
.title-bottom span, .title-bottom-sm span
  align-self: flex-end

.my-card
  width: 100%
  max-width: 250px
  height: 100%
  max-height: 250px

.img-center
  display: block
  margin-left: auto
  margin-right: auto

.product
  margin-left: 30px
  margin-right: 30px
  
.safety
  margin-left: 30px
  margin-right: 30px

@media only screen and (max-width: 600px) 
  .headlines
      font-size: 30px
      text-align: center
  .product
      font-size: 20px
      width: 350px
  .place-order
      font-size: 20px

  .safety
      width:350px
      text-align: left
      font-size: 20px

  .slogan
      font-size: 26px
      margin-left: 30px
      margin-right: 30px
  .list-text
      font-size: 20px

  .contacts
      font-size: 20px
    
  .map
      width: 320px
      height: 300px
      margin-left: 25px

  .icon
      text-align: right

@media only screen and (max-width: 768px) and (min-width: 600px)
  .headlines
      font-size: 30px
      text-align: center
  .product
      font-size: 20px
      width: 600px
  .place-order
      font-size: 20px

  .safety
      width:600px
      text-align: left
      font-size: 20px

  .slogan
      font-size: 26px

  .list-text
      font-size: 20px

  .map
      width: 500px
      height: 400px
      margin-left: 100px

  .icon
      text-align: right

@media only screen and (max-width: 1024px) and (min-width: 768px)
  .headlines
      font-size: 30px
      text-align: center
  .product
      font-size: 20px
      width: 700px
  .place-order
      font-size: 20px

  .safety
      width:700px
      text-align: left
      font-size: 20px

  .slogan
      font-size: 26px

  .list-text
      font-size: 20px

  .map
      width: 550px
      height: 500px
      margin-left: 125px
  .icon
      text-align: right
</style>
