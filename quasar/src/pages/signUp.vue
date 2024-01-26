<template>
  <q-page class="flex flex-center  q-py-xl">
    <div class="glass column q-gutter-y-lg q-pa-xl">
      <h3 class="q-mt-none q-mb-lg text-center text-primary">عضویت</h3>
      <p class="text-center q-my-none">
        قبلا ثبت نام کزده اید ؟ <span class="text-primary">ورود</span>
      </p>
      <q-input standout="bg-primary text-white" label="نام">
        <template v-slot:prepend>
          <q-icon name="person" />
        </template>
      </q-input>
      <q-input standout="bg-primary text-white" label="شماره تلفن">
        <template v-slot:prepend>
          <q-icon name="phone" />
        </template>
      </q-input>
      <q-input standout="bg-primary text-white" label="ایمیل">
        <template v-slot:prepend>
          <q-icon name="mail" />
        </template>
      </q-input>
      <q-input standout="bg-primary text-white" label="رمز عبور">
        <template v-slot:prepend>
          <q-icon name="password" />
        </template>
      </q-input>
      <q-btn class="bg-primary text-white" label="ادامه" />
    </div>
  </q-page>
</template>

<script></script>
