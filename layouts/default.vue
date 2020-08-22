<template>
  <v-app>
    <v-navigation-drawer app clipped>
      <v-list>
        <v-list-item v-for="(item, i) in items" :key="i" :to="item.to" router exact>
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <!-- <v-app-bar app clipped-left flat>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-btn text nuxt to="/">
        <v-toolbar-title v-text="title" />
      </v-btn>
    </v-app-bar>-->

    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <!-- <v-footer app>
      <span>&copy; 2020</span>
    </v-footer>-->
  </v-app>
</template>

<script>
export default {
  props: {
    source: String
  },

  data: () => ({
    drawer: false,
    items: [
      {
        icon: 'mdi-apps',
        title: 'Welcome',
        to: '/'
      },
      {
        icon: 'mdi-cog',
        title: '設定',
        to: '/settings'
      }
    ],
    title: 'Web Design'
  })
}
</script>

<style lang="scss" scoped>
.v-btn {
  text-transform: none;

  &::before {
    background-color: transparent;
  }
}
.theme--light.v-app-bar.v-toolbar.v-sheet {
  background-color: azure;
}
</style>
