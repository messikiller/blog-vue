<template>
  <div>

    <v-container>
      <v-card color="primary">
        <v-card-title class="title white--text">分类</v-card-title>
        <v-list dense>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">list</v-icon></v-list-tile-avatar>
            <v-list-tile-content>cate1</v-list-tile-content>
          </v-list-tile>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">list</v-icon></v-list-tile-avatar>
            <v-list-tile-content>cate1</v-list-tile-content>
          </v-list-tile>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">list</v-icon></v-list-tile-avatar>
            <v-list-tile-content>cate1</v-list-tile-content>
          </v-list-tile>
        </v-list>
      </v-card>
    </v-container>

    <v-container>
      <v-card color="primary">
        <v-card-title class="title white--text">归档</v-card-title>
        <v-list dense>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">date_range</v-icon></v-list-tile-avatar>
            <v-list-tile-content>2018-12-23</v-list-tile-content>
          </v-list-tile>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">date_range</v-icon></v-list-tile-avatar>
            <v-list-tile-content>2018-12-23</v-list-tile-content>
          </v-list-tile>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">date_range</v-icon></v-list-tile-avatar>
            <v-list-tile-content>2018-12-23</v-list-tile-content>
          </v-list-tile>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">date_range</v-icon></v-list-tile-avatar>
            <v-list-tile-content>2018-12-23</v-list-tile-content>
          </v-list-tile>
          <v-list-tile avatar @click="handleClick">
            <v-list-tile-avatar><v-icon color="grey darken-2">date_range</v-icon></v-list-tile-avatar>
            <v-list-tile-content>2018-12-23</v-list-tile-content>
          </v-list-tile>
        </v-list>
      </v-card>
    </v-container>

    <v-container>
      <v-card color="primary" dark>
        <v-card-title class="title">标签云</v-card-title>
        <v-card-text class="white text--primary">
          <v-btn outline color="#3c763d" small round>Outline Button</v-btn>
          <v-btn outline color="indigo" small round>Outline Button</v-btn>
          <v-btn outline color="#3c763d" small round>Outline Button</v-btn>
          <v-btn outline color="indigo" small round>Outline Button</v-btn>
          <v-btn outline color="#3c763d" small round>Outline Button</v-btn>
          <v-btn outline color="indigo" small round>Outline Button</v-btn>
          <v-btn outline color="#3c763d" small round>Outline Button</v-btn>
          <v-btn outline color="indigo" small round>Outline Button</v-btn>
          <v-btn outline color="#3c763d" small round>Outline Button</v-btn>
          <v-btn outline color="indigo" small round>Outline Button</v-btn>
        </v-card-text>
      </v-card>
    </v-container>

  </div>
</template>

<script>
export default {
  methods: {
    handleClick: function () {
      console.log(111)
    }
  }
}
</script>

<style lang="css" scoped>
</style>
