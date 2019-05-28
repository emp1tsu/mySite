<template>
  <v-content class="content-index">
    <v-container fluid>
      <v-layout align-center justify-center>
        <v-flex xs6>
          <v-card>
            <v-layout>
              <v-flex class="pa-4">
                <div>
                  <div class="headline">Skill</div>
                  <ul>
                    <!-- あとでコンポーネント作る星5個中なんこ的な -->
                    <li>JavaScript</li>
                    <li>Vue.js</li>
                    <li>Vuex</li>
                    <li>VueRouter</li>
                    <li>Visual Studio Code</li>
                    <li>English</li>
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
