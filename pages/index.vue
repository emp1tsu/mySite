<template>
  <v-content class="content-index">
    <v-container fluid>
      <v-layout align-center justify-center>
        <v-flex xs6>
          <v-flex class="text-xs-center pa-5">
            <v-avatar size="216">
              <v-img src="https://cdn.vuetifyjs.com/images/cards/foster.jpg" />
            </v-avatar>
          </v-flex>
          <v-card>
            <v-layout>
              <v-flex class="pa-4">
                <div>
                  <div class="headline">基本情報</div>
                  <ul>
                    <li>氏名：高橋涼</li>
                    <li>年齢：22</li>
                    <li>
                      職歴: システムエンジニア - 株式会社アルファシステムズ
                      (2016/04-20xx/xx)
                    </li>
                    <li>
                      はじめまして。22歳SEの高橋涼(@emiptus0813)と申します。
                      社会人3年目です。
                    </li>
                    <li>
                      新卒でSlerに入社し、2年近くWEBアプリ開発に携わり主に
                      クライアントサイドを担当していました。
                      フレームワークはVue.jsを利用しています。
                    </li>
                    <li>
                      お客様と密にコミュニケーションをとりながら仕様決定、製造をし手戻り
                      を少なく作業することができます。また、サーバサイドと連携したフロント
                      エンドの製造をすることができます。
                    </li>
                    <li>
                      他にもソースコードをGHEで管理、PullRequestでのソースコード
                      レビューの経験があります。
                    </li>
                  </ul>
                </div>
              </v-flex>
            </v-layout>
          </v-card>
          <v-card>
            <v-layout>
              <v-flex class="pa-4">
                <div>
                  <div class="headline">スキル</div>
                  <ul>
                    <!-- あとでコンポーネント作る星5個中なんこ的な -->
                    <li>JavaScript</li>
                    <li>Vue.js</li>
                    <li>Vuex</li>
                    <li>VueRouter</li>
                    <li>TypeScript</li>
                    <li>Visual Studio Code</li>
                    <li>English</li>
                  </ul>
                </div>
              </v-flex>
            </v-layout>
          </v-card>
          <v-card>
            <v-layout>
              <v-flex class="pa-4">
                <div>
                  <div class="headline">資格</div>
                  <ul>
                    <li>基本情報技術者</li>
                  </ul>
                </div>
              </v-flex>
            </v-layout>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </v-content>
</template>

<script>
export default {
  data: () => ({
    dark: true,
    drawers: ['Default (no property)', 'Permanent', 'Temporary'],
    primaryDrawer: {
      model: null,
      type: 'default (no property)',
      clipped: false,
      floating: false,
      mini: false
    },
    footer: {
      inset: false
    }
  })
}
</script>

<style scoped>
ul {
  list-style: none;
}
.vimage {
  margin-top: 20px;
}
.content-index {
  z-index: 1;
}
</style>
