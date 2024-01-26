<template>
  <q-layout view="hHh lpr fFf">
    <q-header elevated>
      <q-toolbar>
        <q-toolbar-title>
          <h1 class="text-h6">یوک بار</h1>
        </q-toolbar-title>
        <div class="absolute-center">
          <q-btn to="/" flat color="grey-3" rounded icon="home">
            <q-tooltip class="bg-accent">خانه</q-tooltip>
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

<script></script>
<style>
.glass {
  /* From https://css.glass */
  background: rgba(255, 255, 255, 0.28);
  border-radius: 16px;
  box-shadow: 0 10px 60px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(7px);
  -webkit-backdrop-filter: blur(7px);
  border: 1px solid rgba(248, 247, 247, 0.3);
}
</style>
