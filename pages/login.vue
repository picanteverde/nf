<template>
  <div>
    <TopBar />
    <label>username: </label>
    <input type="text" v-model="name"/>
    <label>password: </label>
    <input type="password" v-model="pass"/>
    <button v-on:click="login">Login</button>
  </div>
</template>

<script>
import TopBar from '~components/TopBar'

export default {
  components: {
    TopBar
  },
  data: () => ({
    name: '',
    pass: ''
  }),
  methods: {
    login: () => {
      alert('login')
    }
  }
}
</script>
