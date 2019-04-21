<template>
  <v-timeline align-top dense class="timeline-with-date">

    <template v-for="(article, index) in articles">
      <v-timeline-item
        icon="rss_feed"
        fill-dot
        :key="index"
      >
      <span class="title font-weight-regular primary--text pubtime">2018-12-23</span>
        <v-card color="primary" dark class="timeline-card">
          <v-card-title class="title">{{ article.title }}</v-card-title>
          <v-card-text class="white text--primary">
            <p>{{ article.content }}</p>
          </v-card-text>
          <v-card-actions class="white grey--text body-1">
            <v-icon color="grey lighten-1" class="subheading">date_range</v-icon>
            <span class="mr-2"> 2018-12-25</span>
            <span class="mr-1">/</span>
            <v-icon color="grey lighten-1" class="subheading">remove_red_eye</v-icon>
            <span class="mr-2"> 256</span>
            <span class="mr-1">/</span>
            <v-icon color="grey lighten-1" class="subheading">list</v-icon>
            <span class="mr-2"> 256</span>
            <span class="mr-1">/</span>
            <v-icon color="grey lighten-1" class="subheading">bookmark_border</v-icon>
            <span class="mr-2"> 256</span>
            <v-spacer />
            <v-btn color="primary" fab>
              <v-icon>search</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-timeline-item>
    </template>

    <v-container>
      <v-layout justify-center>
        <v-pagination v-model="page" :length="8"></v-pagination>
      </v-layout>
    </v-container>
  </v-timeline>
</template>

<script>
export default {
  data () {
    return {
      page: 1,
      articles: [
        {
          title: 'Lorem Ipsum Dolor',
          content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.'
        },
        {
          title: 'Lorem Ipsum Dolor',
          content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.'
        },
        {
          title: 'Lorem Ipsum Dolor',
          content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.'
        },
        {
          title: 'Lorem Ipsum Dolor',
          content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.'
        },
        {
          title: 'Lorem Ipsum Dolor',
          content: 'Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.'
        }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
.timeline-with-date {
  margin-left: 120px;
}
.pubtime {
  position: relative !important;
  left: -180px;
  top: 14px;
}
.timeline-card {
  top: -20px;
}
</style>
