<template>
  <v-container grid-list-md text-xs-center fluid class="grey darken-4 grey--text text--lighten-1">
    <v-layout>
      <v-flex xs6>
        <v-layout align-center justify-center>
          <div style="max-width: 500px;">
            <div class="footer-title white--text">友情链接</div>
            <v-btn outline color="grey" small>阿斯达</v-btn>
            <v-btn outline color="grey" small>阿斯达</v-btn>
            <v-btn outline color="grey" small>阿斯达</v-btn>
            <v-btn outline color="grey" small>阿斯达</v-btn>
            <v-btn outline color="grey" small>阿斯达</v-btn>
            <v-btn outline color="grey" small>阿斯达</v-btn>
            <v-btn outline color="grey" small>阿斯达</v-btn>
          </div>
        </v-layout>
      </v-flex>
      <v-flex xs6>
        <div class="footer-title white--text">打赏支持</div>
        <div class="donate-container">
          <div class="image-item">
            <img class="image-donate" src="https://blog.messikiller.net/images/donate-wechat.jpg" />
            <div class="image-title">微信</div>
          </div>
          <div class="image-item">
            <img class="image-donate" src="https://blog.messikiller.net/images/donate-alipay.jpg" />
            <div class="image-title">支付宝</div>
          </div>
        </div>
      </v-flex>
    </v-layout>
    <div class="line-divider"></div>
    <v-layout>
      <v-divider></v-divider>
      <v-flex xs12 class="white--text">
        Code & Design By Messikiller
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
.footer-title {
  font-size: 1.2em;
  line-height: 2;
  margin-bottom: 15px;
}
.line-divider {
  margin-top: 20px;
  margin-bottom: 20px;
}

.donate-container {
  display: flex;
  justify-content: center;
}

.image-item {
  display: flex;
  flex-direction: column;
}

.image-item:first-child {
  margin-right: 30px;
}

.image-donate {
  height: 150px;
}

.image-title {
  margin-top: 10px;
}
</style>
