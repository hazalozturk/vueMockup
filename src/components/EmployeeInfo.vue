<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <v-flex
        v-for="n in 32"
        :key="n"
        xs3>
        <v-flex mr-4>
        <v-img
          :src="`https://picsum.photos/300/300?image=${n}`"
        ></v-img>
        </v-flex>
        <v-flex mb-4>
          <h1><a
            href=''
            target="_blank">
              Name
          </a></h1>
          <p><a
            href=''
            target="_blank">
              Title
          </a></p>
        </v-flex>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
}
</script>
