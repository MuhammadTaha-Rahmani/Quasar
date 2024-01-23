<template>
  <q-page>
    <div class="row">
      <div class="col text-center">
        <h2 class="text-h4">یوک بار چیست ؟</h2>
        <p>
          لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با
          استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در
          ستون و سطرآنچنان که لازم است، و برای شرایط فعلی تکنولوژی مورد نیاز، و
          کاربردهای متنوع با هدف شصت و سه درصد گذشته حال و آینده، شناخت فرار.
        </p>
      </div>
      <div class="col gt-xs">
        <q-img
          src="../assets/quasar-logo-vertical.svg"
          style="width: 150px; margin: 0 auto; display: block"
        />
      </div>
    </div>
    <q-img src="../assets/wave.svg" style="transform:translateY(1px);"/>
    <div class="bg-secondary q-py-xl">
      <div class="row justify-center q-gutter-lg text-center">
        <div class="col-sm-4 glass">
          <h3 class="text-h4 text-positive q-mb-4">ارتباط مستقیم</h3>
          <p class="text-color">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
            استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در
            ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و
            کاربردهای
          </p>
        </div>
        <div class="col-sm-4 q-mx-2 glass">
          <h3 class="text-h4 text-positive q-mb-4">ارتباط مستقیم</h3>
          <p class="">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
            استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در
            ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و
            کاربردهای
          </p>
        </div>
        <div class="col-sm-5 glass">
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
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>
<style>
.glass {
  /* From https://css.glass */
  background: transparent;
  border-radius: 16px;
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  border: 1px solid rgba(255, 255, 255, 0.3);
}
</style>
