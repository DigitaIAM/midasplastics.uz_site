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
        <q-card class="my-card" v-for="group in groups" :key="group.img" @click="scrollToText(group.ref)">
          <q-img :src="group.img" :ratio="1" style="width:250px">
            <div class="absolute-bottom text-subtitle2 text-center">
              {{ group.title }}
            </div>
          </q-img>
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
        <div class="text-h5" ref="description" id="description" style="padding-left: 150px; padding-right: 150px;"
          label="UF">
          <span class="text-bold">Стаканы c УФ печатью</span> является наиболее распространенным и экономичным
          способом декорирования стаканов. Печать на стаканы производится ультрафиолетовыми красками, прочно
          закрепляющимися на поверхности стакана.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5" ref="description1" id="description1" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Стакан с картонной этикеткой – комбинация пластика и картона.</span> На наружную
          поверхность
          изготовленного полипропиленового стакана наклеивается картонная этикетка.
        </div>
      </div>
    </div>

    <div class="row q-pt-xl">
      <div class="col">
        <div class="text-h5" ref="description2" id="description2" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Стакан с термоусадочной этикеткой.</span> На наружную поверхность полипропиленового
          стакана усаживается термоусадочная этикетка. Печать наносится на внутреннюю поверхность этикетки, благодаря
          чему изображение долго сохраняет свою насыщенность и не истирается.
        </div>
      </div>
    </div>

    <div class="row q-py-xl">
      <div class="col">
        <div class="text-h5" ref="description3" id="description3" style="padding-left: 150px; padding-right: 150px;">
          <span class="text-bold ">Крышки на стаканы.</span> Мы производим полипропиленовые крышки «нахлобучки»
          (поверх крышки для фольги) высокого качества, пригодные для надевания на стакан на высокоскоростных
          разливочных линиях.
        </div>
      </div>
    </div>

    <q-btn icon="shopping_cart" no-caps color="deep-orange" glossy class="text-h4 q-mb-xl" @click="scrollTo()">
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

    <!-- second card -->
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
        <q-img src="product/a1.png" class="img-center q-ma-lg gt-xs" style="width: 100%;" />
      </div>
    </div>

    <!-- price list -->
    <div class="full-width q-py-xl">
      <div class="text-left text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-left: 550px;" ref="ordering">Прайс лист</span>
      </div>
    </div>

    <div>
      <div class="q-pa-md ">
        <q-table title="Стакан с картонной этикеткой 230мл" title-class="text-bold" :rows="rows" :columns="columns"
          row-key="name" hide-bottom />
      </div>

      <div class="q-pa-md">
        <q-table title="Стакан с картонной этикеткой 420мл" title-class="text-bold" :rows="rows_1" :columns="columns_1"
          row-key="name" hide-bottom />
      </div>

      <div class="q-pa-md">
        <q-table title="Стакан с термоусадочной этикеткой 270мл" title-class="text-bold" :rows="rows_2"
          :columns="columns_2" row-key="name" hide-bottom />
      </div>

      <div class="q-pa-md float-left">
        <q-table title="Крышка полипропиленовая" title-class="text-bold" :rows="rows_3" :columns="columns_3"
          row-key="name" hide-bottom />
      </div>
    </div>

    <!-- placing orders -->
    <div class="full-width q-py-xl">
      <div class="text-right text-h3 text-bold text-white">
        <span class="bg-indigo-9 q-pa-md" style="padding-right: 550px;" ref="ordering">Прием заказов</span>
      </div>
    </div>

    <div class="row full-width q-pt-md">
      <div class="col-sm-7 text-center">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3071.069332161991!2d66.93449035323566!3d39.67065494165193!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3f4d19f6d85e60d1%3A0xb4d60d21fc6f24ae!2z0J7QntCeICLQotCe0J3QkyI!5e0!3m2!1sru!2s!4v1673002782281!5m2!1sru!2s"
          width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"></iframe>
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

// price list
// table 1
const columns = [
  {
    name: 'name',
    required: true,
    label: 'Статья затрат/Тираж',
    align: 'left',
    field: (row) => row.name,
    style: 'font-size: 16px',
    headerStyle: {
      fontSize: '1.2em',
      fontWeight: 'bold'
    },
  },
  {
    name: 'a', label: '50 000', field: 'a', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'b', label: '100 000', field: 'b', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'c', label: '150 000', field: 'c', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'd', label: '200 000', field: 'd', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'e', label: '250 000', field: 'e', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'f', label: '300 000', field: 'f', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'g', label: '350 000', field: 'g', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'h', label: '400 000', field: 'h', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
];

const rows = [
  {
    name: 'Цена стакан + крышка, без НДС',
    a: '858,72',
    b: '735,36',
    c: '685,17',
    d: '665,29',
    e: '653,33',
    f: '647,80',
    g: '643,09',
    h: '638,66',
  },
  {
    name: 'Цена стакан + крышка, с НДС',
    a: '961,76',
    b: '823,60',
    c: '767,39',
    d: '745,12',
    e: '731,72',
    f: '725,53',
    g: '720,26',
    h: '715,29',
  },
];

// table 2
const columns_1 = [
  {
    name: 'name',
    required: true,
    label: 'Статья затрат/Тираж',
    align: 'left',
    field: (row) => row.name,
    style: 'font-size: 16px',
    headerStyle: {
      fontSize: '1.2em',
      fontWeight: 'bold'
    }
  },
  {
    name: 'a', label: '50 000', field: 'a', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'b', label: '100 000', field: 'b', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'c', label: '150 000', field: 'c', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'd', label: '200 000', field: 'd', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'e', label: '250 000', field: 'e', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'f', label: '300 000', field: 'f', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'g', label: '350 000', field: 'g', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'h', label: '400 000', field: 'h', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
];

const rows_1 = [
  {
    name: 'Цена стакан + крышка, без НДС',
    a: '1 078,31',
    b: '947,89',
    c: '892,85',
    d: '858,94',
    e: '843,54',
    f: '838,44',
    g: '834,17',
    h: '830,75',
  },
  {
    name: 'Цена стакан + крышка, с НДС',
    a: '1 207,70',
    b: '1 061,63',
    c: '999,99',
    d: '962,01',
    e: '944,76',
    f: '939,05',
    g: '934,27',
    h: '930,44',
  },
];

// table 3
const columns_2 = [
  {
    name: 'name',
    required: true,
    label: 'Статья затрат/Тираж',
    align: 'left',
    field: (row) => row.name,
    style: 'font-size: 16px',
    headerStyle: {
      fontSize: '1.2em',
      fontWeight: 'bold'
    }
  },
  {
    name: 'a', label: '50 000', field: 'a', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'b', label: '100 000', field: 'b', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'c', label: '150 000', field: 'c', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'd', label: '200 000', field: 'd', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'e', label: '250 000', field: 'e', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'f', label: '300 000', field: 'f', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'g', label: '350 000', field: 'g', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
  {
    name: 'h', label: '400 000', field: 'h', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },
];

const rows_2 = [
  {
    name: 'Цена стакан + крышка, без НДС',
    a: '688,12',
    b: '664,60',
    c: '656,76',
    d: '652,84',
    e: '650,49',
    f: '648,92',
    g: '647,80',
    h: '645,22',
  },
  {
    name: 'Цена стакан + крышка, с НДС',
    a: '770,69',
    b: '744,35',
    c: '735,57',
    d: '731,18',
    e: '728,54',
    f: '726,79',
    g: '725,53',
    h: '722,64',
  },
];

// table 4
const columns_3 = [
  {
    name: 'name',
    required: true,
    label: 'Статья затрат/Тираж',
    align: 'left',
    field: (row) => row.name,
    style: 'font-size: 15px',
    headerStyle: {
      fontSize: '1.2em',
      fontWeight: 'bold'
    }
  },
  {
    name: 'a', label: '50 000', field: 'a', style: 'font-size: 15px', headerStyle: {
      fontSize: '1.2em'
    }
  },

];

const rows_3 = [
  {
    name: 'Итого, цена без НДС',
    a: '130,64',
  },
  {
    name: 'Итого, цена с НДС',
    a: '146,31',
  },
];
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


</style>
