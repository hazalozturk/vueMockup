<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <v-flex xs12>
        <h1 class="pb-5 deep-orange--text text-xs-center">{THE TEAM}</h1>
      </v-flex>
      <v-flex
        v-for="employee in employee_list"
        :key="employee.name"
        xs3>
        <v-flex mr-4 pl-3 pb-3>
        <v-img
          :src="employee.image"
        ></v-img>
        </v-flex>
        <v-flex mb-4 pb-3>
          <v-btn
            flat
            :href='employee.url'
            target="_blank">
              {{employee.name}}
          </v-btn>
          <p><a
            class="black--text"
            :href='employee.url'
            target="_blank">
              {{employee.position}}
          </a></p>
        </v-flex>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      employee_list: [
        {
          "url": "https://www.linkedin.com/in/jbriccetti/",
          "position": " CEO ",
          "image": "https://www.troyweb.com/s/Jon.png",
          "name": "Jon Briccetti"
        },
        {
          "url": "https://www.linkedin.com/in/anthonydebonis/",
          "position": " President ",
          "image": "https://www.troyweb.com/s/Anthony.png",
          "name": "Anthony DeBonis"
        },
        {
          "url": "https://www.linkedin.com/in/mark-poskanzer-b694698/",
          "position": "Director of Business Development",
          "image": "https://www.troyweb.com/s/Mark.png",
          "name": "Mark Poskanzer"
        },
        {
          "url": "https://www.linkedin.com/in/chris-m-boyle/",
          "position": " Director of Application Development ",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Chris Boyle"
        },
        {
          "url": "https://www.linkedin.com/in/mike-pacella-42865483/",
          "position": " Senior Developer / Senior Consultant / Project Lead ",
          "image": "https://www.troyweb.com/s/Mike.png",
          "name": "Mike Pacella"
        },
        {
          "url": "https://www.linkedin.com/in/lauren-abbott-749402b7/",
          "position": "Senior Technologist",
          "image": "https://www.troyweb.com/s/Lauren.png",
          "name": "Lauren Abbott"
        },
        {
          "url": "https://www.linkedin.com/in/damian-crisafulli-b484a782/",
          "position": "Senior Developer / Senior Consultant / Project Lead",
          "image": "https://www.troyweb.com/s/Damian.png",
          "name": "Damian Crisafulli"
        },
        {
          "url": "https://www.linkedin.com/in/diane-acosta-b543431a/",
          "position": "Office Manager",
          "image": "https://www.troyweb.com/s/Diane.png",
          "name": "Diane Acosta"
        },
        {
          "url": "https://www.linkedin.com/in/tyler-flood/",
          "position": "Visual Designer",
          "image": "https://www.troyweb.com/s/Tyler.png",
          "name": "Tyler Flood"
        },
        {
          "url": "https://www.linkedin.com/in/jennifer-favitta-pmp-22260717/",
          "position": "Production Manager / Project Manager, PMP",
          "image": "https://www.troyweb.com/s/favitta.png",
          "name": "Jennifer Favitta"
        },
        {
          "url": "https://www.linkedin.com/in/jedidiah-stewart-76008235/",
          "position": " Architect / Senior Developer / Consultant ",
          "image": "https://www.troyweb.com/s/Jed.png",
          "name": "Jedidiah Stewart"
        },
        {
          "url": "https://www.linkedin.com/in/reissa-alderman-688aa1115/",
          "position": "Technologist",
          "image": "https://www.troyweb.com/s/Reissa.png",
          "name": "Reissa Alderman"
        },
        {
          "url": "https://www.linkedin.com/in/ratna-randive-75279385/",
          "position": "Finance Director",
          "image": "https://www.troyweb.com/s/Ratna.png",
          "name": "Ratna Randive"
        },
        {
          "url": "https://www.linkedin.com/in/colin-pitcher-b1179a152/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Colin.png",
          "name": "Colin Pitcher"
        },
        {
          "url": "https://www.linkedin.com/in/kevin-nguyen-78291bb3/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Kevin.png",
          "name": "Kevin Nguyen"
        },
        {
          "url": "https://www.linkedin.com/in/bobbywoodny/",
          "position": "Business Analyst",
          "image": "https://www.troyweb.com/s/Bobby.png",
          "name": "Bobby Wood"
        },
        {
          "url": "https://www.linkedin.com/in/eriksaulnier/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Erik.png",
          "name": "Erik Saulnier"
        },
        {
          "url": "https://www.linkedin.com/in/nataliewysocki/",
          "position": "Interaction Designer",
          "image": "https://www.troyweb.com/s/natalie.jpg",
          "name": "Natalie Wysocki"
        },
        {
          "url": "https://www.linkedin.com/in/stevebadera/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/steve.png",
          "name": "Steve Badera"
        },
        {
          "url": "https://www.linkedin.com/in/kevincoffrin/",
          "position": "Quality Assurance Developer",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Jim O'Keefe"
        },
        {
          "url": "https://www.linkedin.com/in/connor-mcmanus-587834101/",
          "position": " Developer ",
          "image": "https://www.troyweb.com/s/Connor.jpg",
          "name": "Connor McManus"
        },
        {
          "url": "https://www.linkedin.com/in/bengodgart/",
          "position": "Technologist / Data Scientist",
          "image": "https://www.troyweb.com/s/Ben.jpg",
          "name": "Ben Godgart"
        },
        {
          "url": "https://www.linkedin.com/in/nicholaspakatar/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Nick.jpg",
          "name": "Nick Pakatar"
        },
        {
          "url": null,
          "position": "Intern",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Audrey Pitcher"
        },
        {
          "url": "https://www.linkedin.com/in/edwinsvraka/",
          "position": "Technologist",
          "image": "https://www.troyweb.com/s/edwin.jpg",
          "name": "Edwin Svraka"
        },
        {
          "url": "https://www.linkedin.com/in/daniel-wilson-434742105/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Dan.jpg",
          "name": "Daniel Wilson"
        },
        {
          "url": "https://www.linkedin.com/in/adam-bahrani-72b15611a/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Adam.jpg",
          "name": "Adam Bahrani\n"
        },
        {
          "url": "https://www.linkedin.com/in/joseph-iaquinto/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Joe Iaquinto"
        },
        {
          "url": "https://www.linkedin.com/in/timothykeaveny/",
          "position": "Intern",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Tim Keaveny"
        },
        {
          "url": "https://www.linkedin.com/in/joshshea/",
          "position": "Developer",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Josh Shea"
        },
        {
          "url": "https://www.linkedin.com/in/firmin-alexander/",
          "position": "Marketing Specialist",
          "image": "https://www.troyweb.com/s/firmin-a64s.jpg",
          "name": "Firmin Alexander"
        },
        {
          "url": "https://www.linkedin.com/in/tylervorpahl/",
          "position": "Senior Developer",
          "image": "https://www.troyweb.com/s/Owl.png",
          "name": "Tyler Vorpahl"
        }
      ]
    }
  }
}
</script>
