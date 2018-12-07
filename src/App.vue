<template>
  <v-app>
    <Toolbar/>
    <v-content>
      <AboutUs/>
      <EmployeeInfo/>
    </v-content>
    <Footer/>
  </v-app>
</template>

<script>
import EmployeeInfo from './components/EmployeeInfo'
import Toolbar from './components/Toolbar'
import AboutUs from './components/AboutUs'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    EmployeeInfo,
    Toolbar,
    AboutUs,
    Footer
  }
}
</script>
