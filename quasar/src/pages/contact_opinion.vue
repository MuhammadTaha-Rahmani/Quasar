<template>
  <q-page class="my-font">
    <div class="row justify-center q-gutter-y-lg q-my-xl">
      <q-card
        v-for="(message, index) in messages"
        :key="index"
        class="my-card col-7"
        flat
        bordered
      >
        <q-item>
          <q-item-section avatar>
            <q-avatar>
              <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
            </q-avatar>
          </q-item-section>

          <q-item-section>
            <q-item-label>{{
              message.firstName + " " + message.lasttName
            }}</q-item-label>
            <q-item-label caption> {{ message.phoneNum }} </q-item-label>
          </q-item-section>
        </q-item>

        <q-separator />

        <q-card-section horizontal>
          <q-card-section>
            {{ message.message }}
          </q-card-section>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<script>
import { defineComponent, ref } from "vue";
import axios from "axios";
export default defineComponent({
  setup() {
    const messages = ref([]);
    function fetchMessages() {
      axios.get("http://localhost:8000/api/messages").then((r) => {
        console.log(r.data);
        messages.value = r.data;
      });
    }
    fetchMessages();
    return {
      messages,
    };
  },
});
</script>
