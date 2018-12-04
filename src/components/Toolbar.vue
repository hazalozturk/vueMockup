<template>
  <v-toolbar app prominent extended>
      <img src="../assets/logo.png" height="40" class="mt-5">
    <v-spacer></v-spacer>
    <v-toolbar-items v-for="button in toolbar_buttons" class="mt-5">
    <v-btn
      flat
      :href="button.link"
      target="_blank"
    > {{ button.name }}</v-btn>
  </v-toolbar-items>
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
