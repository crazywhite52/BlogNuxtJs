<template>
  <b-container fluid>
    <b-row class="my-1">
      <b-col sm="2">
        <label for="input-small">Small:</label>
      </b-col>
      <b-col sm="5">
        <b-form-input id="input-small" v-model="text1" size="sm" placeholder="Enter your name"></b-form-input>
      </b-col>
      {{text1}}
      <b-button variant="success" @click="addRow(text1)" size="sm">+ Add</b-button>
    </b-row>
    <b-row class="my-1">
      <b-col sm="12">
        <b-alert variant="success" show v-for="(list,index) in lists" :key="index">{{list}}</b-alert>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  layout: 'coreLayout',
  data() {
    return {
      lists: [],
      text1: '',
      text1: ''
    }
  },
  methods: {
    addRow(e) {
      this.lists.push(e)
      this.text1 = "";
    }
  }
}
</script>