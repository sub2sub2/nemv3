<template>
  <v-container grid-list-md text-xs-center>
    <v-layout row wrap>
      <v-flex xs12 sm6 md4 lg3 xl2>
      <v-card color="red">
        a
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 md4 lg3 xl2>
      <v-card color="blue">
        b
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 md4 lg3 xl2>
      <v-card color="red">
        c
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 md4 lg3 xl2>
      <v-card color="blue">
        d
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 md4 lg3 xl2>
      <v-card color="red">
        e
      </v-card>
    </v-flex>
    <v-flex xs12 sm6 md4 lg3 xl2>
      <v-card color="blue">
        f
      </v-card>
    </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'about',
  data () {
    return {
      ta: 'debug'
    }
  },
  mounted () {
    this.ta = JSON.stringify(this.$vuetiry.breakpoint)
  }

}
</script>
