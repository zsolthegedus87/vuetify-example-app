<template>
  <v-container>
    <v-row v-if="loading">
      <v-col sm="12" md="4">
        <v-card class="pa-4">
          <v-skeleton-loader type="heading"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="heading"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="paragraph@2"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="chip" tile="tile"></v-skeleton-loader>
        </v-card>
      </v-col>
      <v-col sm="12" md="4">
        <v-card class="pa-4">
          <v-skeleton-loader type="heading"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="heading"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="paragraph@2"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="chip" tile="tile"></v-skeleton-loader>
        </v-card>
      </v-col>
      <v-col sm="12" md="4">
        <v-card class="pa-4">
          <v-skeleton-loader type="heading"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="heading"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="paragraph@2"></v-skeleton-loader>
          <br />
          <v-skeleton-loader type="chip" tile="tile"></v-skeleton-loader>
        </v-card>
      </v-col>
    </v-row>
    <v-row v-else>
      <v-col sm="12" md="4">
        <v-card class="fill-height" max-width="344">
          <v-card-title>Card Title 1</v-card-title>
          <v-card-subtitle>Card Sub-title 1</v-card-subtitle>
          <v-card-text
            >A tálos pedelek a plások alatt szongatnak meg, de csak a fagyalás
            első darosán. Ezek általában elég gyógyító talákat szilágyítnak,
            ezért talt az izmusa. Hasonlóan a plásokhoz, a felék szeszti el.
          </v-card-text>
          <v-card-actions>
            <v-btn text>Button 1</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col sm="12" md="4">
        <v-card class="fill-height" max-width="344">
          <v-card-title>Card Title 1</v-card-title>
          <v-card-subtitle>Card Sub-title 1</v-card-subtitle>
          <v-card-text
            >A felék általában a fagyalás lonk fagyos elsője, ő likálja, és
            lózja karban. Az egész fagyaláshoz latozódzhatik, és rágozhatja,
            például takákat pesedhetik, kodhatik elsőket, egyzéreket ringizálhat
            létre.
          </v-card-text>
          <v-card-actions>
            <v-btn text>Button 2</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col sm="12" md="4">
        <v-card class="fill-height" max-width="344">
          <v-card-title>Card Title 1</v-card-title>
          <v-card-subtitle>Card Sub-title 1</v-card-subtitle>
          <v-card-text
            >A szaplat csápság hazásban disztalan matos folyóka. Szagos
            seleszmerések illetve a sidáshoz bákos jáció velő ide kattintva.
            Háklyás szegzés, 4-5 parárra rendkívül verő törgés.
          </v-card-text>
          <v-card-actions>
            <v-btn text>Button 3</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      loading: false,
    };
  },
  mounted() {
    this.loading = true;
    setTimeout(() => {
      this.loading = false;
    }, 5000);
  },
};
</script>
