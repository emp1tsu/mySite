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
                  <div class="headline">About Me</div>
                  <ul>
                    <li>氏名：高橋涼</li>
                    <li>年齢：22</li>
                    <li>
                      はじめまして。22歳SEの高橋涼(@emiptus0813)と申します。
                      社会人3年目です。
                    </li>
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
