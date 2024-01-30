<template>
  <q-layout view="hHh lpr fFf">
    <q-header elevated>
      <q-toolbar class="my-font bg-white text-light-blue-8">
        <q-toolbar-title>
          <h1 class="text-h6">یوک بار</h1>
        </q-toolbar-title>
        <div class="absolute-center">
          <q-btn
            v-for="nav in navs"
            :to="nav.to"
            flat
            class="gt-xs"
            color="light-blue-4"
            rounded
            :icon="nav.icon"
            :key="nav.key"
          >
            <q-tooltip class="bg-blue-8 shadow-10">{{nav.tooltip}}</q-tooltip>
          </q-btn>
        </div>

        <div>
          <q-btn icon="person" />
          <q-btn icon="person" />
        </div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, reactive } from "vue";
export default defineComponent({
  setup() {
    const navs = reactive([
      {
        icon: "home",
        tooltip: "خانه",
        to: "/",
        key: "1",
      },
      {
        icon: "work",
        tooltip: "کار",
        to: "/signup",
        key: "2",
      },{
        icon: "message",
        tooltip: "گفت و گو",
        to: "/opinion",
        key: "3",
      }
    ]);
    return {
      navs,
    };
  },
});
</script>
<style>
.glass {
  /* From https://css.glass */
  background: rgba(255, 255, 255, 0.28);
  border-radius: 16px;
  /* box-shadow: 0 10px 60px rgba(0, 0, 0, 0.1); */
  backdrop-filter: blur(7px);
  -webkit-backdrop-filter: blur(7px);
  border: 1px solid rgba(248, 247, 247, 0.3);
}
</style>
