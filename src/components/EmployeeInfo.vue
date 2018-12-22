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
        xs12 md4 lg3>
        <v-flex mr-4 pl-3 pb-3>
        <v-avatar size="16em">
          <v-img
          class="elevation-20"
          :src="employee.image"
          ></v-img>
        </v-avatar>
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
import axios from 'axios'

export default {
  data() {
    return {
      employee_list: []
    }
  },
  created: function () {
    this.getEmployeeList()
  },
  methods: {
    getEmployeeList: function () {
      var vm = this
      axios.get('https://gist.githubusercontent.com/hazalozturk/c1da3e671c2989dac850e6ecac54983f/raw/98423fb779d43d139d2ab355872ade2741e15ade/employee.json')
        .then(function (response) {
          vm.employee_list = response.data
        })
    }
  }
}
</script>
