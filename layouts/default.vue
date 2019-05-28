<template>
  <v-app id="sandbox">
    <v-toolbar :clipped-left="primaryDrawer.clipped" app absolute>
      <v-toolbar-title>empitsuについて</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn to="/" flat>About me</v-btn>
        <v-btn to="/career" flat>Career</v-btn>
        <v-btn to="/skill" flat>Skill</v-btn>
        <v-btn to="/certificate" flat>Certificate</v-btn>
        <v-btn to="/contact" flat>Contact</v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <nuxt />
    <v-footer :inset="footer.inset" app>
      <span class="px-3">&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
    <vue-particles
      class="background"
      color="#696969"
      :particleOpacity="0.7"
      :particlesNumber="80"
      shapeType="circle"
      :particleSize="4"
      linesColor="#696969"
      :linesWidth="1"
      :lineLinked="true"
      :lineOpacity="0.4"
      :linesDistance="150"
      :moveSpeed="3"
      :hoverEffect="true"
      hoverMode="grab"
      :clickEffect="true"
      clickMode="push"
    >
    </vue-particles>
  </v-app>
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
a {
  text-decoration: none;
}

a:link {
  color: rgba(0, 0, 0, 0.87);
}

.background {
  position: absolute;
  display: block;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
}
</style>
