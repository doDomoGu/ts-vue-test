<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button v-on:click="hello">Click</button>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HelloWorld extends Vue {
  @Prop() /* private */ msg!: string
  created() {
    console.log(2, 3, 4)
  }
  hello() {
    console.log('say hello')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
