<template>
    <v-app-bar
      style="padding: 0 90px"
      app
      color="white"
      light
      elevation="6"
      elevate-on-scroll
    >
      <v-toolbar-title class="brand">
        Alexanyer Naranjo
      </v-toolbar-title>
      <v-spacer />
      <v-list class="d-flex align-center">
        <v-list-item link v-for="(item, index) in menuItems" :key="index">
          <v-list-item-title>{{item}}</v-list-item-title>
        </v-list-item>
        <v-btn text>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
        <v-btn outlined color="indigo">Get Started</v-btn>
      </v-list>
    </v-app-bar>  
</template>

<script>
export default {
    name: 'NavBar',
    data () {
        return {
            menuItems: [
                'Home',
                'About Me',
                'Portfolio',
                'Projects',
                'Gallery',
                'Contact'
            ]
        }
    }
}
</script>

<style>
.brand
{
  font-size: 32px;
  color: #1565C0;
  font-weight: 700;
}
</style>
