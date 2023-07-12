<template>
    <v-tabs
      v-model="tab"
      color="deep-purple-accent-4"
      align-tabs="center"
    >
      <v-tab value="one">Welcome</v-tab>
      <v-tab value="two">About Me</v-tab>
      <v-tab value="three">Mini-projects</v-tab>
      <v-tab value="four">Art Gallery</v-tab>
      <v-tab value="five">Contact Me</v-tab>
    </v-tabs>

    <v-card-text>
      <v-window v-model="tab">
        <v-window-item value="one">
          <HomePage/>
        </v-window-item>

        <v-window-item value="two">
          Two
        </v-window-item>

        <v-window-item value="three">
          <Miniprojects/>
        </v-window-item>
      </v-window>
    </v-card-text>

</template>

<script setup>
  import HomePage from '@/views/Home.vue'
  import Miniprojects from '@/views/Miniprojects.vue'
</script>
<script>
  export default {
    data: () => ({
      tab: null,
    }),
  }
</script>