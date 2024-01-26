<template>
  <q-page>
    <div class="row q-my-xl">
      <div class="col text-center">
        <h2 class="text-h3 text-primary">یوک بار چیست ؟</h2>
        <p>
          لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با
          استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در
          ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و
          کاربردهای متنوع با هدف شصت و سه درصد گذشته حال و آینده، شناخت فرار.
        </p>
      </div>
    </div>
    <q-img src="../assets/wave.svg" style="transform: translateY(1px)" />
    <div class="bg-secondary q-py-xl">
      <h3 class="text-center q-mt-none q-mb-xl text-positive">
        راهنمای استفاده
      </h3>
      <div class="row justify-center q-gutter-lg text-center">
        <div class="col-sm-5  col-11 q-pa-md glass">
          <h3 class="text-h4 text-positive q-mb-4">ارتباط مستقیم</h3>
          <p class="text-color">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
            استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در
            ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و
            کاربردهای
          </p>
        </div>
        <div class="col-sm-5 col-11 q-mx-2 q-pa-md glass">
          <h3 class="text-h4 text-positive q-mb-4">ارتباط مستقیم</h3>
          <p class="">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
            استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در
            ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و
            کاربردهای
          </p>
        </div>
        <div class="col-sm-5 col-11 q-pa-md glass">
          <h3 class="text-h4 text-positive q-mb-4">ارتباط مستقیم</h3>
          <p class="text-color">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
            استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در
            ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و
            کاربردهای
          </p>
        </div>
      </div>
    </div>
    <div
      class="row text-primary justify-center text-center q-py-lg q-gutter-xl justify-center"
    >
      <div
        :key="sectionIcon.key"
        v-for="sectionIcon in sectionIcons"
        class="glass q-pa-lg col-10 col-sm-4 "
      >
        <q-icon :name="sectionIcon.name" size="60px" />
        <p class="text-h5 text-indigo-5">{{ sectionIcon.title }}</p>
        <p :data-goal="sectionIcon.goal" class="text-h4 text-weight-regular">
          0
        </p>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent, reactive } from "vue";

export default defineComponent({
  name: "IndexPage",
  setup() {
    const sectionIcons = reactive([
      {
        name: "person",
        goal: "10",
        title: "کاربران فعال",
        key: "1",
      },
      {
        name: "star",
        goal: "14",
        title: "رضایت کاربران",
        key: "2",
      },
      {
        name: "mail",
        goal: "52",
        title: "نظرات",
        key: "3",
      },
      {
        name: "favorite",
        goal: "123",
        title: "کاربران راضی",
        key: "4",
      },
    ]);
    return {
      sectionIcons,
    };
  },
});
</script>
