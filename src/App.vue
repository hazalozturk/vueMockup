<template>
  <v-app>
    <v-content>
      <EmployeeInfo/>
    </v-content>
  </v-app>
</template>

<script>
import EmployeeInfo from './components/EmployeeInfo'

export default {
  name: 'App',
  components: {
    EmployeeInfo
  }
}
</script>
