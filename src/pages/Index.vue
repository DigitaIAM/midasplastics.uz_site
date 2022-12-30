<template>
  <q-page class="flex flex-center" style="background: white;">
    <!-- title -->
    <div class="full-width q-pb-xl">
      <div class="row full-width">
        <div class="col-sm-2 bg-indigo-9">
        </div>
        <div class="col-sm-3">
          <q-img src="/logo.png" class="float-center q-ma-lg gt-xs" style="max-width: 70%; height: auto" />
        </div>
        <div class="col-sm-7 text-justtify text-h2 text-bold text-red q-py-xl">
          ПРАВИЛЬНАЯ УПАКОВКА
          <br />
          ДЛЯ ПРАВИЛЬНЫХ ПРОДУКТОВ
        </div>
      </div>
    </div>

    <div class="full-width q-pt-lg">
      <div class="text-right text-h3 text-bold title-top text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-right: 400px;">НАШЕ ПРОИЗВОДСТВО</span>
      </div>
    </div>

    <!-- <h1>
      <a href="/Quasar/quasar_demo/quasar-midasplastics/src/pages/Index.vue/#c1">
        Link
      </a>
    </h1> -->

    <h1>
      <a href="#c1">
        Link
      </a>
    </h1>

    <router-link v-bind:to="'/Quasar/quasar_demo/quasar-midasplastics/src/pages/Index.vue/#c1'" class='primary'>GOOO
    </router-link>
    <!-- description -->
    <!-- first card -->
    <div class="row full-width q-pt-lg flex-center">
      <div class="col-sm-6">
        <q-img src="tools/1.png" class="img-center q-ma-lg q-ml-xl" style="width: 80%;" />
      </div>
      <div class="col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left">
          <div class="q-pa-md">
            оснащено лучшим в мире <br /> оборудованием европейского производства
          </div>
        </div>
      </div>
    </div>
    <!-- second card -->
    <div class="row full-width q-pt-md flex-center">
      <div class="col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left">
          <div class="q-pa-md">
            обеспечивает высокую производительность
          </div>
        </div>

      </div>
      <div class="col-sm-6">
        <q-img src="tools/2.png" class="img-center q-mr-lg q-mr-xl" style="width: 80%; " />
      </div>
    </div>
    <!-- third card -->
    <div class="row full-width q-pt-lg flex-center">
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

      <div class="col-sm-6">
        <div class="row q-px-lg q-pt-lg text-h5 text-left ">
          <div class="q-pa-md">
            позволяет производить широкий ассортимент <br />стаканов различных форм и объемов без <br />значительных
            инвестиций в дорогостоящие пресс-формы
          </div>
        </div>
      </div>
    </div>

    <div class="full-width q-pt-lg">
      <div class="text-left text-h3 text-bold title-top text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-left: 400px;">КАЧЕСТВО И БЕЗОПАСНОСТЬ</span>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" style="padding-left: 150px; padding-right: 150px;">
          Все наше производство устроено так, как если бы мы производили детское питание - это позволяет нам
          гарантировать чистоту и безопасность нашей продукции.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <q-img src="product/a4.jpg" class="img-center q-ma-lg gt-xs" style="width: 650px; height: auto;" />
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" style="padding-left: 150px; padding-right: 150px;">
          Начиная от полимерной гранулы и заканчивая готовой упаковкой с декором - мы отслеживаем качество упаковки всех
          стадиях производства. Это позволяет нам выпускать достойный продукт со стабильным качеством.
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

    <!-- products -->
    <div class="full-width q-py-xl">
      <div class="text-right text-h3 text-bold title-top text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-right: 600px;">ПРОДУКЦИЯ</span>
      </div>
    </div>



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

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" id="c1" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold" id="c1">Стаканы c печатью</span> является наиболее распространенным и экономичным
          способом декорирования стаканов. Печать на стаканы производится ультрафиолетовыми красками, прочно
          закрепляющимися на поверхности стакана.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" id="c2" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Стакан с картонной этикеткой – комбинация пластика и картона.</span> На наружную
          поверхность
          изготовленного полипропиленового стакана наклеивается картонная этикетка.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" id="c3" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Стакан с термоусадочной этикеткой.</span> На наружную поверхность полипропиленового
          стакана усаживается термоусадочная этикетка. Печать наносится на внутреннюю поверхность этикетки, благодаря
          чему изображение долго сохраняет свою насыщенность и не истирается.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5 text-justify" id="c4" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Крышки на стаканы.</span> Мы производим полипропиленовые крышки «нахлобучки»
          (поверх крышки для фольги) высокого качества, пригодные для надевания на стакан на высокоскоростных
          разливочных линиях.
        </div>
      </div>
    </div>

    <!-- placing orders -->
    <div class="full-width q-py-xl">
      <div class="text-left text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-left: 550px;">ПРИЕМ ЗАКАЗОВ</span>
      </div>
    </div>

    <div class="row full-width flex-center q-pt-md">
      <div class="col-sm-7 text-center">
        <q-img src="location/geo.png" class="img q-ma-lg gt-xs" style="height:fit-content; width: 50%;" />
      </div>

      <div class="col-sm-5">
        <div class="q-pa-md" style="max-width: 400px">
          <div class="row">
            <div class="col-sm-1 text-primary text-h6"><span class="material-icons">phone
              </span></div>
            <div class="col-sm-11 text-h6"><a href="tel:+998 93 333 85 75" style="color: darkorchid;">
                +998 93 333 85 75
              </a> <br />
              <a href="tel:+998 93 720 33 38" style="color: darkorchid;">
                +998 93 720 33 38
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

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "PageIndex",
  setup() {
    return {
      slide: ref('first'),
      groups: [
        { img: "product/a5.jpg", title: "Cтакан с УФ печатью", id: "1" },
        { img: "product/a6.jpg", title: "Стакан с картонной этикеткой", id: "2" },
        { img: "product/a7.jpg", title: "Стакан с термоусадочной этикеткой", id: "3" },
        { img: "product/a8.jpg", title: "Крышки на стаканы", id: "4" },
      ],
    }
  }
});




</script>
<style lang="sass" scoped>
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
