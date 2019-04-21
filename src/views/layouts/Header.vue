<template>
  <v-toolbar dark fixed color="primary">
    <v-avatar
      size="40"
      color="grey lighten-4"
    >
      <img src="https://blog.messikiller.net/images/header-logo.jpg" alt="avatar">
    </v-avatar>
    <v-toolbar-title>Messikiller's Blog | <span class="subheading font-weight-regular">折而不挠，终不为下</span></v-toolbar-title>
    <v-layout align-center justify-end row fill-height>
      <v-toolbar-items class="hidden-sm-and-down">

        <v-menu offset-y v-for="(cate, pIdx) in cates" :key="pIdx" open-on-hover>
          <template v-slot:activator="{ on }">
            <v-btn dark flat v-on="on">
              {{ cate.title }}
              <v-icon v-if="cate.subs">arrow_drop_down</v-icon>
            </v-btn>
          </template>
          <v-list v-if="cate.subs">
            <v-list-tile v-for="(sub, sIdx) in cate.subs" :key="sIdx">
              <v-list-tile-title>{{ sub.title }}</v-list-tile-title>
            </v-list-tile>
          </v-list>
        </v-menu>

      </v-toolbar-items>
    </v-layout>
  </v-toolbar>
</template>

<script>
export default {
  data () {
    return {
      cates: [
        {
          title: '前端',
          subs: [
            { title: 'HTML/CSS' },
            { title: 'JavaScript' }
          ]
        },
        {
          title: '后台',
          subs: [
            { title: 'PHP' },
            { title: 'Golang' },
            { title: 'Shell' }
          ]
        },
        {
          title: '运维',
          subs: [
            { title: 'Linux' },
            { title: 'Windows' },
            { title: 'Network' }
          ]
        },
        {
          title: '数据库',
          subs: [
            { title: 'MySQL' },
            { title: 'Redis' },
            { title: 'Memcache' }
          ]
        },
        { title: '随笔' }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
