<template>
  <q-page class="flex flex-center">
    <q-btn icon="download" color="light-blue-4" rounded class="q-px-xl" outline push>Download</q-btn>
    <q-input prefix="+98" rounded outlined label="phone" />
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>
