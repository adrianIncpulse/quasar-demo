<template>
  <q-page class="bg-grey-12">
    <q-responsive :ratio="16 / 9" style="max-height: 100vh">
      <q-carousel animated v-model="slide" arrows navigation infinite>
        <q-carousel-slide
          :name="1"
          img-src="https://cdn.quasar.dev/img/mountains.jpg"
        />
        <q-carousel-slide
          :name="2"
          img-src="https://cdn.quasar.dev/img/parallax1.jpg"
        />
        <q-carousel-slide
          :name="3"
          img-src="https://cdn.quasar.dev/img/parallax2.jpg"
        />
        <q-carousel-slide
          :name="4"
          img-src="https://cdn.quasar.dev/img/quasar.jpg"
        />
        <q-carousel-slide :name="0" :img-src="imageOmnilife" />
      </q-carousel>
    </q-responsive>

    <q-responsive :ratio="16 / 9" style="max-height: 100vh" class="q-mt-xl">
      <div class="row fit justify-center items-center">
        <div class="col-10 bg-white shadow-1" style="border: 1px solid #fdfdfd">
          <div class="row full-width">
            <div style="width: 50%" class="q-pa-md q-pl-lg">HOLA OMNIPLUS</div>
            <div style="width: 50%">
              <q-img :src="omniplus" />
            </div>
          </div>
        </div>
      </div>
    </q-responsive>

    <q-responsive :ratio="16 / 9" style="max-height: 100vh">
      <div class="row fit justify-center items-center">
        <div class="col-10 bg-white shadow-1" style="border: 1px solid #fdfdfd">
          <div class="row full-width">
            <div style="width: 50%">
              <q-img :src="aqtua" />
            </div>
            <div style="width: 50%" class="q-pa-md q-pl-lg">HOLA AQTUA</div>
          </div>
        </div>
      </div>
    </q-responsive>

    <q-responsive :ratio="16 / 9" style="max-height: 100vh">
      <div class="row fit justify-center items-center">
        <div class="col-10 bg-white shadow-1" style="border: 1px solid #fdfdfd">
          <div class="row full-width">
            <div style="width: 50%">
              <q-img :src="power" />
            </div>
            <div style="width: 50%" class="q-pa-md q-pl-lg">HOLA MUNDO</div>
          </div>
        </div>
      </div>
    </q-responsive>
  </q-page>
</template>

<script setup>
import { ref } from "vue";
import imageOmnilife from "src/assets/banners/omni.jpg";
import power from "src/assets/productos/power.png";
import omniplus from "src/assets/productos/omniplus.jpg";
import aqtua from "src/assets/productos/aqtua.jpg";

const slide = ref(0);
</script>
