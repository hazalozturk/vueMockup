<template>
  <v-toolbar app prominent>
      <img src="../assets/logo.png" height="40">
    <v-spacer></v-spacer>
    <v-toolbar-items v-for="button in toolbar_buttons" class="hidden-sm-and-down">
    <v-btn
      flat
      :href="button.link"
      target="_blank"
    > {{ button.name }}</v-btn>
  </v-toolbar-items>
  <v-menu large class="hidden-md-and-up">
    <v-btn
      slot="activator"
      color="orange" fab dark
    >
      <v-icon large>list</v-icon>
    </v-btn>
    <v-list>
      <v-list-tile
        v-for="button in toolbar_buttons"
        :href="button.link"
        :key="button.name"
        target="_blank"
      > <v-list-tile-title>
          {{ button.name }}
        </v-list-tile-title>
      </v-list-tile>
    </v-list>
  </v-menu>
  </v-toolbar>
</template>

<script>
export default {
  data () {
    return {
      toolbar_buttons: [
        {
          name: 'ABOUT US',
          link: 'https://www.troyweb.com/about-us/'
        },
        {
          name: 'SERVICES',
          link: 'https://www.troyweb.com/custom-software-development/'
        },
        {
          name: 'CLIENTS',
          link: 'https://www.troyweb.com/clients/'
        },
        {
          name: 'CAREERS',
          link: 'https://www.troyweb.com/careers/'
        },
        {
          name: 'CONTACT',
          link: 'https://www.troyweb.com/contact/'
        }
      ]
    }
  }
}
</script>
