<template>
  <q-page class="flex flex-center" style="background: #f5f7f5;">
    <!-- title -->
    <div class="full-width header">
      <div class="title text-center text-h3 text-bold title-top text-red q-pb-xl">
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
    <div class="row full-width">
      <div class="col-sm-8">
        <q-img src="tools/1.png" class="img-center q-ma-lg gt-xs"
          style="width: 100%;" />
      </div>
      <div class="col-sm-4">
        <div class="row q-px-lg q-pt-lg text-h6 text-left">
          оснащено лучшим в мире <br /> оборудованием европейского производства
        </div>
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

