<template>
  <v-app>
    <Toolbar/>
    <v-content>
      <EmployeeInfo/>
    </v-content>
  </v-app>
</template>

<script>
import EmployeeInfo from './components/EmployeeInfo'
import Toolbar from './components/Toolbar'

export default {
  name: 'App',
  components: {
    EmployeeInfo,
    Toolbar
  }
}
</script>
