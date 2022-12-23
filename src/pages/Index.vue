<template>
  <q-page class="flex flex-center" style="background: #f5f7f5;">
    <!-- title -->
    <div class="full-width header">
      <div class="title text-center text-h3 text-bold title-top text-red q-pa-xl">
        ПРАВИЛЬНАЯ УПАКОВКА
        <br />
        ДЛЯ ПРАВИЛЬНЫХ ПРОДУКТОВ
      </div>
      <div class="title text-center text-h4 text-bold title q-pb-lg q-ma-lg">
        <span>
          Мы производим пищевую упаковку для молочных предприятий.
        </span>
      </div>
      <div class="title text-center text-h3 text-bold title-top text-white ">
        <span class="bg-positive q-pa-md">НАШЕ ПРОИЗВОДСТВО</span>
      </div>
    </div>


    <!-- description -->
    <!-- first card -->
    <div class="row full-width q-pt-lg flex-center">
      <div class="col-sm-7">
        <q-img src="tools/1.png" class="img-center q-ma-lg gt-xs" style="width: 90%;" />
      </div>
      <div class="col-sm-5">
        <div class="row q-px-lg q-pt-lg text-h5 text-left">
          <div class="q-pa-md">
            <q-card style="max-width: 500px">
              <q-card-section>
                <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" rect fill="red" class="bi bi-circle-fill"
                  viewBox="0 0 16 16">
                  <circle cx="8" cy="8" r="8" />
                </svg> оснащено лучшим в мире <br /> оборудованием европейского производства
              </q-card-section>
            </q-card>
          </div>
        </div>
        <q-separator />
      </div>
    </div>
    <!-- second card -->
    <div class="row full-width q-pt-md flex-center">
      <div class="col-sm-5">
        <div class="row q-px-lg q-pt-lg text-h5 text-left">
          <div class="q-pa-md">
            <q-card style="max-width: 500px">
              <q-card-section>
                <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" rect fill="red" class="bi bi-circle-fill"
                  viewBox="0 0 16 16">
                  <circle cx="8" cy="8" r="8" />
                </svg> обеспечивает высокую производительность
              </q-card-section>
            </q-card>

          </div>
        </div>
        <q-separator />
      </div>
      <div class="col-sm-7">
        <q-img src="tools/2.png" class="img-center q-mr-lg gt-xs" style="width: 90%;" />
      </div>
    </div>
    <!-- third card -->
    <div class="row full-width flex-center q-pt-lg">
      <div class="col-sm-7 flex-center">
        <div class="row">
          <div class="col-sm-4"></div>
          <div class="col-sm-4">
            <q-img src="product/a1.jpg" class="img-center q-ma-lg gt-xs" style="width: 90%;" />
          </div>
          <div class="col-sm-4"></div>
        </div>
        <div class="row">
          <div class="col-sm-3">
          </div>
          <div class="col-sm-3">
            <q-img src="product/a2.jpg" class="img-center q-ma-lg gt-xs" style="width: 90%;" />
          </div>
          <div class="col-sm-3">
            <q-img src="product/a3.jpg" class="img-center q-ma-lg gt-xs" style="width: 90%;" />
          </div>
          <div class="col-sm-3">
          </div>

        </div>
      </div>

      <div class="col-sm-5">
        <div class="row q-px-lg q-pt-lg text-h5 text-left  ">
          <div class="q-pa-md">
            <q-card style="max-width: 500px">
              <q-card-section>
                <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" rect fill="red" class="bi bi-circle-fill"
                  viewBox="0 0 16 16">
                  <circle cx="8" cy="8" r="8" />
                </svg> позволяет производить широкий ассортимент стаканов различных форм и объемов без значительных
                инвестиций в дорогостоящие пресс-формы
              </q-card-section>
            </q-card>
          </div>
        </div>
        <q-separator />
      </div>
    </div>



  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageIndex",
});
</script>

