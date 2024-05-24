<template>
  <q-layout>
    <div class="q-pa-md">

      <q-header class="header">w
        <q-toolbar>
          <q-btn flat round dense icon="menu" class="q-mr-sm" />
          <q-avatar>
            <img src="https://media.discordapp.net/attachments/1235900412062601269/1243535956037079040/1670068.png?ex=6651d49b&is=6650831b&hm=1a10df0e007900546dfddac278a19ca85ae9b473bfb5525e99f5083865826c06&=&format=webp&quality=lossless"> 
          </q-avatar>

          <q-toolbar-title>Flower Bloom Shop</q-toolbar-title>

          <q-btn flat round dense icon="local_florist" />
        </q-toolbar>

        <q-tabs v-model="tab">
          <q-tab name="home" label="Home" />
          <q-tab name="promo" label="Promo" />
          <q-tab name="about" label="About Us" />
        </q-tabs>
      </q-header>
      <q-page-container>
        <q-page class="q-pa-md">

 <!-- Carousel -->
      <div class="q-pa-md">
          <q-carousel
            v-model="slide"
            transition-prev="slide-right"
            transition-next="slide-left"
            swipeable
            animated
            control-color="black"
            navigation
            padding
            arrows
            height="300px"
          >
            <q-carousel-slide :name="1" class="column no-wrap">
              <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
                <q-img class="rounded-borders col-6 full-height" src="https://img.freepik.com/free-vector/watercolor-spring-social-media-promo-template_23-2149286028.jpg?t=st=1716551220~exp=1716551820~hmac=0b45df5096f526e5db9832256156ca0a629bcf399221ab1e95b775ef1cef80f0" />
                <q-img class="rounded-borders col-6 full-height" src="https://img.freepik.com/free-vector/flat-spring-social-media-cover-template_23-2149257356.jpg?w=1800&t=st=1716552669~exp=1716553269~hmac=46845686eef4a64efd42088c7208da5b5242512589787f5e6734c1d0cc03e723" /> 
              </div>
            </q-carousel-slide>
            <q-carousel-slide :name="2" class="column no-wrap">
              <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
                <q-img class="rounded-borders col-6 full-height" src="https://img.freepik.com/free-vector/florist-sale-banner-template-design_23-2150173303.jpg?t=st=1716552772~exp=1716556372~hmac=1399ec17412dbe3e1f199100e118fccbedceb3fb564609a86317262995601a57&w=1380" />
                <q-img class="rounded-borders col-6 full-height" src="https://img.freepik.com/free-vector/flat-spring-sale-horizontal-banner_23-2149260723.jpg?t=st=1716553256~exp=1716556856~hmac=cf68734d5f4f9779ae70c492317d498ef8a59b62a607336f6d8c7f67fe1c6804&w=1380" /> 
              </div>
            </q-carousel-slide>
            <q-carousel-slide :name="3" class="column no-wrap">
              <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
                <q-img class="rounded-borders col-6 full-height" src="https://img.freepik.com/free-photo/amorous-couple-with-passionate-red-rose_23-2147738219.jpg?t=st=1716552880~exp=1716556480~hmac=0b9f06d55e4c5dc0754f8a535ce5180cb3d7f5607f5663ad3278aabbd463bc0e&w=1380" /> 
                <q-img class="rounded-borders col-6 full-height" src="https://i.pinimg.com/564x/0b/51/c8/0b51c8c11f51cd1df46e31700d7eaab9.jpg" /> 
              </div>
            </q-carousel-slide>
          </q-carousel>
        </div>
<!-- End of Carousel -->

      <div class="kategori">
        <div class="q-pa-md row items-start q-gutter-md">
          <!-- Flower Categories -->
          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/2e/97/b6/2e97b644053b26055a5075d26d163fa2.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Tulip <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              The tulip is a perennial bulbous plant belonging to the genus Tulipa, which is part of the Liliaceae family.  <!--deskripsi dari bunga-->
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/90/27/79/902779514510bf5b9fb0d516db7ab1bd.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Rose <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              Rose is a flowering plant belonging to the genus Rosa in the family Rosaceae. Roses have been cultivated for thousands of years.
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/01/1d/05/011d05e28f2a3438e9b95f572f131331.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Peonies <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              Peonies are perennial flowering plants belonging to the genus Paeonia in the family Paeoniaceae. 
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/01/1e/02/011e02b5a7b4c5ed63fa40f32862fe8f.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Lily  <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              Lilies are flowering plants belonging to the genus Lilium in the family Liliaceae and have six petal-like segments arranged.
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/31/4c/bd/314cbda14889b15f6592ef5efea6ae0b.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Camellia <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              Camellia is a genus of flowering plants in the family Theaceae, native to eastern and southern Asia. <!--deskripsi dari bunga-->
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/a1/f1/70/a1f170d1083e38a9a7837d0cb74eac83.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Sweet Pea <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              The sweet pea (Lathyrus odoratus) is a flowering plant in the legume family Fabaceae, native to Sicily, Cyprus, southern Italy.
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/77/1a/1f/771a1fa59beaf1068b6dbe13621921f8.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Orchids <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              Orchids are one of the largest and most diverse families of flowering plants, known as Orchidaceae. 
            </q-card-section>
          </q-card>

          <q-card class="my-card">
            <q-img class="bunga" src="https://i.pinimg.com/564x/96/7d/22/967d226c4b99811da9b30d66f99259a0.jpg"> <!--GANTI-->
              <div class="absolute-bottom text-h6">
                Custom Flower <!--nama bvunga-->
              </div>
            </q-img>

            <q-card-section>
              You can custom and request flower here. <!--deskripsi dari bunga-->
            </q-card-section>
          </q-card>
        </div>
      </div>
        <!-- End of Product Cards -->

        </q-page>
      </q-page-container>
    </div>
    <q-footer reveal elevated class="footer">
        <q-toolbar>
          <q-toolbar-title>Serlina Siregar</q-toolbar-title>
        </q-toolbar>
      </q-footer>

    
  </q-layout>
</template>

<script>
export default {
  data() {
    return {
      tab: 'home',
      slide: 'slide1',
      lorem: 'A beautiful selection of flowers for all occasions.'
    };
  }
}
</script>

<style>

.header {
  background-color: #ffc0cb;
}

.q-carousel {
  background-color: #ffc0cb; 
}
.footer {
  background-color: #ffc0cb; 
  text-align: center; 
}

.my-card {
  background-color: #ffc0cb;
  color: black; 
}

.my-card .text-h6 {
  color: white;
}
.store-card {
  width: 300px;
}
.image-container {
  height: 200px;
}
.image {
  height: 100%;
  object-fit: cover;
}
.centered {
  justify-content: center;
}

.bunga {
  width: 252.97px;
  height: 337.43px;
  border-radius: 15px;
}
.my-card {
  width: 252.97px;
  height: 450px;
  text-align: center
  
}

.kategori {
  display: flex;
  justify-content: center; /* Posisikan konten secara horizontal di tengah */
}

/* Card Container */
.q-pa-md.row.items-start.q-gutter-md {
  display: flex;
  flex-wrap: wrap;
  justify-content: center; /* Posisikan card secara horizontal di tengah */
}
</style>
