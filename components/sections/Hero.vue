<template>
  <!-- home page rolling -->
  <section id="hero">
    <v-carousel
      height="calc(100vh - 64px)"
      dark
      cycle
      show-arrows-on-hover
      draggable="true"
      hide-delimiter-background
    >
      <v-carousel-item
        v-for="(carousel, carindex) in carouselsData"
        :key="carindex"
        :src="carousel.src"
        class="gradient-fill"
      >
        <v-container fill-height>
          <div style="max-width: 600px">
            <div
              class="text-md-h2 mb-3 text-sm-h3 text-h5 font-weight-black white--text"
            >
              {{ carousel.heading.toUpperCase() }}
            </div>
            <p class="mb-5 white--text">{{ carousel.subHeading }}</p>
            <v-btn :x-large="$vuetify.breakpoint.smAndUp" class="my-3 primary"
              >Quick Start</v-btn
            >
            <span class="mx-2 my-4"></span>
            <!-- <v-btn
              :x-large="$vuetify.breakpoint.smAndUp"
              text
              class="my-3"
              outlined
              dark
              ><v-icon left large color="primary">mdi-play</v-icon>Learn
              More</v-btn
            > -->
          </div>
        </v-container>
      </v-carousel-item>
    </v-carousel>
  </section>
</template>

<script>
export default {
  data() {
    return {
      carouselsData: [
        {
          src: 'pexels-andrea-piacquadio-3884440.jpg',
          heading: ' Build your model with our service ',
          subHeading:
            ' SynSpot pptimize your AI model cooperatively with others without sharing data and model.',
        },
        {
          src: 'pexels-peter-olexa-4012966.jpg',
          heading: ' PROMOTE YOUR BUSINESS WITH US',
          subHeading:
            'SynSpot brings together millions of data science practitioners, data-driven enterprises, and the open source community.',
        },
        {
          src: 'pexels-thirdman-5961072.jpg',
          heading: ' TACKLE YOUR CHALLENGE',
          subHeading:
            'SynSpot solutions are serious technology for real data science and ML applications. You will be ready to solve problems in your daily life.',
        },
        {
          src: 'pexels-andrea-piacquadio-3830745.jpg',
          heading: ' OWN YOUR DESTINY ',
          subHeading:
            'SynSpot is an open-source innovation which can keep pace with your needs and business challenges',
        },
      ],
    }
  },
}
</script>

<style>
.gradient-fill .v-responsive__content {
  background: rgb(0, 0, 0);
  background: linear-gradient(
    to right,
    rgba(3, 12, 41, 0.75),
    rgba(5, 11, 31, 0.65)
  );
}
</style>
