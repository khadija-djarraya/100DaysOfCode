<template>
    <div>
      <v-hover v-slot="{ isHovering, props }">
        <v-card
        class="mx-auto"
        max-width="300"
        variant="outlined"
        style="left: auto; right: auto; position: relative; margin: 10px; padding: 0px; border-radius: 0px; border: 0px; box-shadow: none;"
        v-bind="props"
        >
          <v-img
            :src="image"
            height="200px"
          >
            <v-expand-transition>
              <div
                v-if="isHovering"
                class="d-flex transition-fast-in-fast-out bg-purple-darken-2 v-card--reveal text-h3"
                style="height: 100%;"
              >
              {{ projectTitle }}
              </div>
            </v-expand-transition>
          </v-img>
        </v-card>
      </v-hover>
    </div>
  </template>
  <style>
    .v-card--reveal {
      align-items: center;
      bottom: 0;
      justify-content: center;
      opacity: .9;
      position: absolute;
      width: 100%;
    }
</style>
<script>
    export default {
        name: "MyCard",
      props: {
        image: {
          type: String,
          required: true,
        },
        projectTitle: {
          type: String,
          required: true,
        },
      },
    };
  </script>