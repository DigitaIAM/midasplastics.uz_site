<template>
  <q-page class="flex flex-center" style="background: #f5f7f5;">
    <!-- title -->
    <div class="full-width top-img header">
      <div class="title text-left text-h3 text-bold title-top q-pt-xl q-pl-xl">
        <q-img src="/logo.svg" style="width: 15vw; height: auto" />
      </div>
      <div class="title text-center text-h4 text-bold title-bottom full-width q-pa-md">
        <span class="full-width">
          Правильная упаковка для правильных продуктов
        </span>
      </div>
    </div>

    <!-- products -->
    <div class="row text-h6 text-center full-width q-ma-lg">
      <div class="fit row wrap justify-center content-center q-gutter-xl">
        <q-card class="my-card" v-for="group in groups" :key="group.img">
          <a href="#c1"><q-img :src="group.img" :ratio="1" style="width:250px">
              <div class="absolute-bottom text-subtitle2 text-center">
                {{ group.title }}
              </div>
            </q-img>
          </a>
        </q-card>
      </div>
    </div>

    <div class="full-width q-py-lg">
      <div class="text-right text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-right: 600px;">Продукция</span>
      </div>
    </div>

    <div class="row q-py-lg">
      <div class="col">
        <div class="text-h5 first" id="c1" style="padding-left: 150px; padding-right: 150px;" label="UF">
          <span class="text-bold">Стаканы c УФ печатью</span> является наиболее распространенным и экономичным
          способом декорирования стаканов. Печать на стаканы производится ультрафиолетовыми красками, прочно
          закрепляющимися на поверхности стакана.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5" id="c2" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Стакан с картонной этикеткой – комбинация пластика и картона.</span> На наружную
          поверхность
          изготовленного полипропиленового стакана наклеивается картонная этикетка.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5" id="c3" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Стакан с термоусадочной этикеткой.</span> На наружную поверхность полипропиленового
          стакана усаживается термоусадочная этикетка. Печать наносится на внутреннюю поверхность этикетки, благодаря
          чему изображение долго сохраняет свою насыщенность и не истирается.
        </div>
      </div>
    </div>

    <div class="row q-py-xl">
      <div class="col">
        <div class="text-h5" id="c4" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Крышки на стаканы.</span> Мы производим полипропиленовые крышки «нахлобучки»
          (поверх крышки для фольги) высокого качества, пригодные для надевания на стакан на высокоскоростных
          разливочных линиях.
        </div>
      </div>
    </div>

    <q-btn icon="shopping_cart" no-caps color="deep-orange" glossy class="text-h4  q-mb-xl" @click="scrollTo()">
      Оформить заказ
    </q-btn>

    <!-- quality & safety -->
    <div class="full-width q-pt-lg">
      <div class="text-left text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-left: 400px;">Качество и безопасность</span>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" style="padding-left: 150px; padding-right: 150px;">
          <q-img src="product/a4.jpg" class="q-ml-xl float-right" style="width: 600px; height: auto;" />
          Все наше производство устроено так, как если бы мы производили детское питание - это позволяет нам
          гарантировать чистоту и безопасность нашей продукции. Начиная от полимерной гранулы и заканчивая готовой
          упаковкой с декором - мы отслеживаем качество упаковки всех стадиях производства. Это позволяет нам выпускать
          достойный продукт со стабильным качеством.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h4 text-center text-indigo-9 text-bold" style="padding-left: 300px; padding-right: 300px;">
          ООО «MIDAS PLASTICS» - это производство полного цикла
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" style="padding-left: 150px; padding-right: 150px;">
          Весь путь от гранулы до готовой упаковки с печатью полностью проходит на одной территории, что позволяет нам
          отслеживать весь процесс и производить качественный продукт.</div>
      </div>
    </div>

    <!-- tools -->
    <div class="full-width q-pt-xl">
      <div class="text-right text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-right: 400px;">Наше производство</span>
      </div>
    </div>

    <!-- description -->
    <!-- first card -->
    <div class="row full-width q-pt-lg flex-center">
      <div class="col-sm-6">
        <q-img src="tools/1.png" class="img-center q-ma-lg q-ml-xl" style="width: 80%;" />
      </div>
      <div class="col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left">
          <div class="col-1 text-right">
            ✔&nbsp;
          </div>
          <div class="col">
            оснащено лучшим в мире оборудованием европейского производства
          </div>
        </div>
        <div class="row q-px-lg q-pt-lg text-h5">
          <div class="col-1 text-right">
            ✔&nbsp;
          </div>
          <div class="col">
            обеспечивает высокую производительность
          </div>
        </div>
      </div>
    </div>

    <!-- third card -->
    <div class="row full-width q-pt-lg flex-center">
      <div class="col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left ">
          <div class="col-1 text-right">
            ✔&nbsp;
          </div>
          <div class="col">
            позволяет производить широкий ассортимент стаканов различных форм и объемов без <br />значительных
            инвестиций в дорогостоящие пресс-формы
          </div>
        </div>
      </div>

      <div class="col-sm-6 flex-center">
        <div class="row">
          <div class="col-sm-4"></div>
          <div class="col-sm-4">
            <q-img src="product/a1.jpg" class="img-center q-ma-lg gt-xs" style="width: 100%;" />
          </div>
          <div class="col-sm-4"></div>
        </div>
        <div class="row">
          <div class="col-sm-3">
          </div>
          <div class="col-sm-3">
            <q-img src="product/a2.jpg" class="img-center q-ma-lg gt-xs" style="width: 100%;" />
          </div>
          <div class="col-sm-3">
            <q-img src="product/a3.jpg" class="img-center q-ma-lg gt-xs" style="width: 100%;" />
          </div>
          <div class="col-sm-3">
          </div>
        </div>
      </div>
    </div>

    <!-- placing orders -->
    <div class="full-width q-py-xl">
      <div class="text-left text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-left: 550px;" ref="ordering">ПРИЕМ ЗАКАЗОВ</span>
      </div>
    </div>

    <div class="row full-width q-pt-md">
      <div class="col-sm-7 text-center">
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3071.069332161991!2d66.93449035323566!3d39.67065494165193!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3f4d19f6d85e60d1%3A0xb4d60d21fc6f24ae!2z0J7QntCeICLQotCe0J3QkyI!5e0!3m2!1sru!2s!4v1673002782281!5m2!1sru!2s" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>

      <div class="col-sm-5">
        <div class="q-pa-md" style="max-width: 400px">
          <div class="row">
            <div class="col-sm-1 text-primary text-h6"><span class="material-icons">phone
              </span></div>
            <div class="col-sm-11 text-h6"><a href="tel:+998933338575" style="color: darkorchid;">
                +998 93 333-85-75
              </a> <br />
              <a href="tel:+998937203338" style="color: darkorchid;">
                +998 93 720-33-38
              </a>
            </div>
          </div>
        </div>
        <div class="q-pa-md" style="max-width: 400px">
          <div class="row">
            <div class="col-sm-1 text-primary text-h6"><span class="material-icons">place
              </span></div>
            <div class="col-sm-11 text-h6">Узбекистан, г. Самарканд, ул. Гагарина, 36.
            </div>
          </div>
        </div>
        <div class="q-pa-md" style="max-width: 400px">
          <div class="row">
            <div class="col-sm-1 text-primary text-h6"><span class="material-icons">mail
              </span></div>
            <div class="col-sm-11 text-h6"><a href="mailto:info@midasplastics.uz">info@midasplastics.uz</a>
            </div>
          </div>
        </div>
      </div>

    </div>
  </q-page>
</template>

<script setup>
import { defineComponent, ref } from "vue";
import { scroll } from 'quasar'
const { getScrollTarget, setVerticalScrollPosition } = scroll

const slide = ref('first');
const groups = [
  { img: "product/a5.jpg", title: "Cтакан с УФ печатью", id: "1" },
  { img: "product/a6.jpg", title: "Стакан с картонной этикеткой", id: "2" },
  { img: "product/a7.jpg", title: "Стакан с термоусадочной этикеткой", id: "3" },
  { img: "product/a8.jpg", title: "Крышки на стаканы", id: "4" },
]

const ordering = ref(null)
const scrollTo = () => {
  const el = ordering.value
  const target = getScrollTarget(el)
  const offset = el.offsetTop
  const duration = 300
  setVerticalScrollPosition(target, offset, duration)
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

.custom-caption
  text-align: center
  padding: 12px
  color: white
  background-color: rgba(0, 0, 0, .3)

.my-card
  width: 100%
  max-width: 250px
  height: 100%
  max-height: 250px

.img-center
  display: block
  margin-left: auto
  margin-right: auto

</style>
