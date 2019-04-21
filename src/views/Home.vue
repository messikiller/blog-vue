<template>
  <div>
    <Header />
    <v-container grid-list-md style="padding-top: 64px; padding-bottom: 0;">
      <v-layout>
        <v-flex xs8>
          <Content />
        </v-flex>
        <v-flex xs4>
          <Sider />
        </v-flex>
      </v-layout>
    </v-container>

    <Footer />
  </div>
</template>

<script>
import Header from '@/layouts/Header'
import Content from '@/layouts/Content'
import Sider from '@/layouts/Sider'
import Footer from '@/layouts/Footer'

export default {
  components: {
    Header,
    Content,
    Sider,
    Footer
  },
  data () {
    return {

    }
  }
}
</script>
