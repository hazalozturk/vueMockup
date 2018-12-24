<template>
  <v-container fluid px-0 py-0 text-xs-center grid-list-md>
    <v-flex xs12 grey lighten-3>
      <img src="../assets/banner.jpg">
    </v-flex>
    <v-flex xs12>
      <h1 class="orange--text text--accent-3 mt-4 text-xs-center font-weight-bold">
        { ABOUT  TROY WEB CONSULTING }
      </h1>
      <h3 class="orange--text text--accent-2 font-weight-medium">
        Our Mission Is To Design And Build Kick-Ass Software.
      </h3>
    </v-flex>
    <v-timeline>
     <v-timeline-item
       color="orange accent-3"
       large
     >
       <span slot="opposite" class="font-weight-medium">In 2002</span>
       <v-card class="elevation-10 rounded-card">
         <v-card-text class="text-xs-right">
           Troy Web Consulting formed from a small band of software
           developers in New York's Capital District who had convened around
           various rapid application development tools that were beginning to
           define the agile web.
         </v-card-text>
       </v-card>
     </v-timeline-item>
     <v-timeline-item
       color="orange accent-3"
       large
     >
       <span slot="opposite"></span>
       <v-card class="elevation-10 rounded-card">
         <v-card-text class="text-xs-left">
           Distinguished by a diverse group of talented,
           business-savvy designers, developers, & consultants, our goal was
           simple: to bring the agility and power of rapid application
           development to businesses and government, provide the best
           customer service in the marketplace and create an engaging,
           rewarding workplace.
         </v-card-text>
       </v-card>
     </v-timeline-item>
     <v-timeline-item
       color="orange accent-3"
       large
     >
       <span slot="opposite" class="font-weight-medium">Now</span>
       <v-card class="elevation-10 rounded-card">
         <v-card-text class="text-xs-right">
           More than 15 years later, our mission lives on.
           Troy Web Consulting is proud to be the area's recognized leader in
           Custom Software Development, Experiential Design, Integration &
           Modernization and Consulting & Strategy.         </v-card-text>
       </v-card>
     </v-timeline-item>
    </v-timeline>
    <v-flex xs12>
      <h2 class="orange--text text--accent-3 py-4 font-weight-bold">
        { OUR CORE VALUES }
      </h2>
      <v-layout justify-center row wrap>
        <v-flex xs2 v-for="value in core_values">
          <v-flex>
          <v-img
            :src="value.icon"
          ></v-img>
          </v-flex>
          <v-flex>
            <p class="font-weight-bold grey--text">
              {{value.info}}
            </p>
          </v-flex>
        </v-flex>
      </v-layout>
    </v-flex>
    <v-flex py-5 xs12 grey darken-2 white--text>
      <h1 class="orange--text text--accent-3 pb-4 text-xs-center font-weight-bold">
        { TECHNOLOGY }
      </h1>
      <p>
        PHP, C#, .NET, Javascript, Java, Node.js, Titanium, ColdFusion,
        AngularJS, React, Vue.js, jQuery, HTML5, CSS, <br> Cordova, MySQL,
        MS SQL Server, MongoDB & Elasticsearch.
      </p>
      <h2 pt-3>Frameworks, Standards & Tools</h2>
      <p>
        Laravel, .NET MVC Framework, .NET Core, Java Spring Framework,
        Grails, Ionic, Express, Bootstrap, <br> Foundation, TeamCity, Selenium,
        Jenkins & Git.
      </p>
      <h2 pt-3>Don't be afraid to ask</h2>
      <p>
        We work with all kinds of technology everyday - Alexa, Siri,
        Raspberry Pi; We've been doing all kinds of IoT <br> device integration
        for years: solar panel monitors, museum display case monitors,
        internet enabled padlocks <br> and cameras.
      </p>
      </p>
    </v-flex>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      core_values: [
        {
          icon:'https://static1.squarespace.com/static/593ad95da5790a81949b5613/t/5bec5658898583febaffd9a9/1542215260295/CoreValues-01-min.png?format=300w',
          info:'Be Agile, Flexible and Lean'
        },
        {
          icon:'https://static1.squarespace.com/static/593ad95da5790a81949b5613/t/5bec566640ec9a4b55d1ebc1/1542215277529/CoreValues-04-min.png?format=300w',
          info:'Embrace Change'
        },
        {
          icon:'https://static1.squarespace.com/static/593ad95da5790a81949b5613/t/5bec56741ae6cf499c60da68/1542215292529/CoreValues-02-min.png?format=300w',
          info:'Pay Attention to Details'
        },
        {
          icon:'https://static1.squarespace.com/static/593ad95da5790a81949b5613/t/5bec568421c67c90311b61d6/1542215307872/CoreValues-03-min.png?format=300w',
          info:'Lead by Example'
        },
        {
          icon:'https://static1.squarespace.com/static/593ad95da5790a81949b5613/t/5bec56930e2e72982defdf07/1542215322567/CoreValues-05-min.png?format=300w',
          info:'Give Back'
        },
        {
          icon:'https://static1.squarespace.com/static/593ad95da5790a81949b5613/t/5bec56a0898583febaffde1f/1542215335469/CoreValues-06-min.png?format=300w',
          info:'Kick-Ass and Take Names'
        }
      ]
    }
  }
}
</script>

<style>
.rounded-card{
    border-radius:30px;
}
</style>
