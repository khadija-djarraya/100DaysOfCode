<template>
<v-col cols="4" sm="6" md="4">
    <v-card
      class="mx-auto"
      variant="outlined"
      style="border: ;"
      height="250px"
    >
      <v-card-item>
        <div>
          <div class="text-overline mb-1">
            OVERLINE
          </div>
          <div class="text-h6 mb-1">
            Headline
          </div>
          <div class="text-caption">Greyhound divisely hello coldly fonwderfully</div>
        </div>
      </v-card-item>
    </v-card>
  </v-col>
</template>
<style>

    .v-card{
        border-radius: 50px;
        box-shadow: 0px 0px 10px 0px rgb(55, 53, 57);    }
</style>

<script>
    export default {
        name: "MyCard2",
      props: {
      }
    };
</script>