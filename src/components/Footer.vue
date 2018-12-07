<template>
  <v-footer
    color="grey darken-2"
    height="auto"
  >
    <v-layout
      justify-center
      row
      wrap
    >
      <v-btn
        v-for="icon in icon_list"
        :key="icon"
        class="mx-3 white--text"
        icon
      >
        <v-icon size="24px">{{ icon }}</v-icon>
      </v-btn>
      <v-flex
        grey
        darken-2
        py-3
        text-xs-center
        white--text
        xs12
      >
        <v-flex pl-5 text-xs-left xs12><p><a  href="https://www.troyweb.com/blog">View Blog →</a></p></v-flex>
        <v-btn
          v-for="item in footer_menu_items"
          :key="item.name"
          color="white"
          flat
          :href="item.link"
          target="_blank"
        > {{ item.name }}</v-btn>
        <p class="white--text pt-5">
          (518) 326-3798 | 200 Broadway, Troy NY 12180 | sales@troyweb.com<br>
          <br>
          Development Center: 5 Third Street, 2nd Floor Troy NY <br>
          <br>
          Community Incubator: 291 River Street, 2nd Floor Troy NY 12180
        </p>
        </v-flex>
        <v-flex
          deep-orange
          py-5
          text-xs-center
          white--text
          xs12
        >
        <h3>
          { CUSTOM SOFTWARE DEVELOPED IN TROY, NEW YORK }
        </h3>
      </v-flex>
    </v-layout>
  </v-footer>
</template>

<script>
export default{
  data () {
    return {
      footer_menu_items: [
        {
          link: 'https://www.troyweb.com/home',
          name: 'HOME'
        },
        {
          link: 'https://www.troyweb.com/about-us',
          name: 'ABOUT US'
        },
        {
          link: 'https://www.troyweb.com/services',
          name: 'SERVICES'
        },
        {
          link: 'https://www.troyweb.com/clients',
          name: 'CLIENTS'
        },
        {
          link: 'https://www.troyweb.com/career',
          name: 'CAREERS'
        },
        {
          link: 'https://www.troyweb.com/community',
          name: 'COMMUNITY'
        },
        {
          link: 'https://www.troyweb.com/contact',
          name: 'CONTACT'
        }
      ],
      icon_list: [
        'home',
        'event',
        'info',
        'folder'
      ]
    }
  }
}
</script>
