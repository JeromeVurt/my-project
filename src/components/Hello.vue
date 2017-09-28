<template>
  <div class="hello">
    <input type="input" class="form-control item" id="exampleInputEmail1" placeholder="UserName" v-model="userName">
    <input type="password" class="form-control item" id="exampleInputPassword1" placeholder="Password" v-model="password">
    <button type="button" class="btn btn-lg btn-primary" @click="login">Logining</button>
  </div>
</template>

<script>

import axios from 'axios'
import { API_URL } from '../config/config.js'

export default {
  data () {
    return {
      userName: '',
      password: ''
    }
  },

   methods: {
      login() {
        if (this.userName && this.password) {
          axios.post(`${API_URL}/rbac/login/${this.userName}?password=${this.password}`, {username: this.userName, password: this.password}).then(d => {
            console.log(d)
          })
        }
      }
   },

  mounted() {
    // console.log(API_URL)
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
.item {
  width: 50%;
  margin: 0 auto;
  margin-bottom: 20px;
}
</style>
