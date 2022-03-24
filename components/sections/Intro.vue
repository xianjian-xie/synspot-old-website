<template>
  <section id="intro" class="py-16">
    <v-container>
      <v-responsive class="max-auto mx-auto text-center" max-width="600">
        <v-avatar color="primary" size="70" class="mb-8">
          <v-icon x-large dark>mdi-web</v-icon>
        </v-avatar>
        <h2 class="text-h4 text-md-h3 text-center font-weight-black mb-7">
          The Perfect Application for Beginners or Professionals
        </h2>
        <p class="title font-weight-light">
          SynSpot — is a carefully crafted multi-purpose, responsive, and
          gorgeous application built with
          <strong>Vue.js</strong>
          and
          <strong>Python</strong>. It comes with the features you need to
          quickly start your data analysis, optimize your AI model cooperatively
          with others without sharing local data.
        </p>
      </v-responsive>

      <v-row class="pt-12">
        <v-col v-for="card in cards" :key="card.title" cols="12" md="4">
          <v-row no-gutters>
            <v-col :cols="card.callout ? 9 : 12">
              <div class="pr-2">
                <div class="text--disabled" v-text="card.subtitle"></div>
                <h4
                  class="text-uppercase mt-1 mb-4"
                  style="letter-spacing: 0.15em"
                  v-text="card.title"
                ></h4>
                <p v-text="card.text"></p>
              </div>
            </v-col>
            <v-col v-if="card.callout" cols="2">
              <span
                class="text-h3 grey--text font-weight-bold pr-8"
                style="opacity: 0.1"
                >{{ card.callout }}</span
              >
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          title: 'Best Productivity',
          subtitle: 'Professionally developed',
          text: 'All components and features are developed using the most up-to-date coding practices.',
          callout: '01',
        },
        {
          title: 'Fast & Low Cost',
          subtitle: 'Performance',
          text: 'SynSpot offers fast Decentralized Machine Learning as a service at a lower cost.',
          callout: '02',
        },
        {
          title: 'Collaborative',
          subtitle: 'Motivation',
          text: 'SynSpot enables easier collaboration across organizations from various industries without sharing sensitive data',
          callout: '03',
        },
      ],
    }
  },
}
</script>
