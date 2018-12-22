<template>
  <v-footer
    color="grey darken-2"
    height="auto"
  >
    <v-layout
      justify-center
      wrap
    >
    <v-flex v-for="text in footer_texts" :key="text.parag" py-5 xs4>
       <h2 class="pb-5 text-xs-center deep-orange--text "> { {{text.title}} }</h2>
       <h3 class="pl-4 white--text pb-3">{{text.subtitle}}</h3>
       <p class="pl-4 white--text">
         {{text.parag}}
         <br><br>
         Read More →
       </p>
    </v-flex>
    <v-flex xs12><v-btn flat color="white" target="_blank" href="https://www.troyweb.com/blog">View Blog →</v-btn></v-flex>
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
        <h2>
          { CUSTOM SOFTWARE DEVELOPED IN TROY, NEW YORK }
        </h2>
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
      footer_texts: [
        {
            title: "BLOG",
            subtitle: "WHY DO YOU NEED A CODE REVIEW?",
            parag: "When your potential or current consumer browses your \
             website, uses your application, submits an online form or \
             completes a purchase with their credit or debit card, they have \
             an expectation that their personal information is transferred and\
             stored securely. Protecting your consumer begins with the \
             foundation of your website or application...your code. Verifying\
             that your code is secure safeguards your consumers and helps\
             ensure that your business is protected against cyber attacks."
        },
        {
          title: "NEWS",
          subtitle: "19TH ANNUAL RESOURCEFUL WOMEN'S AWARDS LUNCHEON",
          parag: "YWCA of the Greater Capital Region, Inc. announces Nathaalie\
            Carey, Deputy Commissioner for Administration and Chief Financial \
            Officer at NYS Department of Labor, as the 2018 Resourceful Woman \
            of the Year.  The event, presented by Groff Networks and Troy Web \
            Consulting, will be held Monday, November 19, 2018 at the Albany \
            Marriott (new location), 11:30a.m. to 1:30p.m."
        },
        {
          title: "TWITTER",
          subtitle: "something something",
          parag: "this need twitter API key and get real data from their page"
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
