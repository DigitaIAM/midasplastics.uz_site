<template>
  <q-layout view="hHh lpR fFf">

    <q-header elevated class="bg-indigo-9 text-white">
      <q-toolbar>
        <q-toolbar-title>
          Midas Plastics
        </q-toolbar-title>
        <div class="text-h6"><a href="tel:+998 93 333 85 75" style="color: white;">
            +998 93 333 85 75
          </a></div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <!-- <q-footer elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>
          <div>Contacts</div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer> -->

  </q-layout>
</template>

<script>

import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  setup() {
    return {}
  },
});
</script>
