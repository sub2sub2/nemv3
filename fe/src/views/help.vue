<template>
  <div>
    <h1>{{title}}</h1>
    <button @click="test">test</button>
    <v-btn :color="btnColor" @click="test">test</v-btn>
    <v-chip close color="primary">Example Chip</v-chip>
    <v-chip v-for="chip in chips" :color="chip.cl" v-bind:key="chip">{{chip.name}}</v-chip>
  </div>
</template>

<script>

export default {
  name: 'help',
  data () {
    return {
      title: 'Vuetify.js',
      btnColor: 'success',
      chips: [
        {
          cl: 'primary',
          name: 'aaaaa'
        },
        {
          cl: 'secondary',
          name: 'bbbbb'
        },
        {
          cl: 'green',
          name: 'ccccc'
        },
        {
          cl: 'warning',
          name: 'dddd'
        }
      ]
    }
  },
  methods: {
    test () {
      this.title = 'nnnnnnn'
      this.btnColor = 'warning'
    }
  }
}
</script>
