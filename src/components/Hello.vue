<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li><a href="https://vuejs.org" target="_blank">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank">Twitter</a></li>
      <br>
      <li><a href="http://vuejs-templates.github.io/webpack/" target="_blank">Docs for This Template</a></li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
    <div>
      <!-- Standard button -->
      <button type="button" class="btn btn-default">（默认样式）Default</button>

      <!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
      <button type="button" class="btn btn-primary">（首选项）Primary</button>

      <!-- Indicates a successful or positive action -->
      <button type="button" class="btn btn-success">（成功）Success</button>

      <!-- Contextual button for informational alert messages -->
      <button type="button" class="btn btn-info">（一般信息）Info</button>

      <!-- Indicates caution should be taken with this action -->
      <button type="button" class="btn btn-warning">（警告）Warning</button>

      <!-- Indicates a dangerous or potentially negative action -->
      <button type="button" class="btn btn-danger">（危险）Danger</button>

      <!-- Deemphasize a button by making it look like a link while maintaining button behavior -->
      <button type="button" class="btn btn-link">（链接）Link</button>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },

  mounted() {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
h1, h2 {
  font-weight: normal;
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
