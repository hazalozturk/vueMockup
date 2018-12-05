<template>
  <v-app>
    <Toolbar/>
    <v-content>
      <AboutUs/>
      <EmployeeInfo/>
    </v-content>
  </v-app>
</template>

<script>
import EmployeeInfo from './components/EmployeeInfo'
import Toolbar from './components/Toolbar'
import AboutUs from './components/AboutUs'

export default {
  name: 'App',
  components: {
    EmployeeInfo,
    Toolbar,
    AboutUs
  }
}
</script>
