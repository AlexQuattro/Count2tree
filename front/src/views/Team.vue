<template>
  <v-content>
    <h1>La Team</h1>

    <v-card v-for="n in 2" :key="n" class="mx-auto" max-width="434" tile>
      <v-col cols="6">
        <v-row>
          <v-avatar class="profile" color="grey" size="164" tile>
            <v-img :src="img.name"></v-img>
          </v-avatar>
        </v-row>
      </v-col>
    </v-card>
  </v-content>
</template>

<script>
export default {
  name: "Team",
  data: () => ({
    img: (
    { name: require("../assets/aless.png") },
    { name: require("../assets/coco.png") })
  })
};
</script>