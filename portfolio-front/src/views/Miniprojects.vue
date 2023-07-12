<template>
<v-row>
    <v-col cols="9" sm="6" md="4">
      <MyCard
        image="https://picsum.photos/350/215"
        project-title="Youtube Downader"
      />
    </v-col>
    <v-col cols="9" sm="6" md="4">
      <MyCard
        image="https://picsum.photos/350/214"
        project-title="NLP Project: Text to bullet points"
      />
    </v-col>
    <v-col cols="9" sm="6" md="4">
      <MyCard
        image="https://picsum.photos/350/216"
        project-title="Deep Learning"
      />
    </v-col>
    <v-col cols="9" sm="6" md="4">
      <MyCard
        image="https://picsum.photos/350/217"
        project-title="Scrape data from website"
      />
    </v-col>
  </v-row>
</template>
<script setup>
import MyCard from '@/components/mycard.vue'
</script>
<script>
export default {
  name: 'Miniprojects',
  components: {
    MyCard,
  },
}
</script>