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

<script>

</script>
