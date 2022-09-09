<template>
<div>
  <h1>Hello vue</h1>
<!--  <my-user v-for='user in users'
  :name='user.name'
  :description='user.description'
  :is-active='user.isActive' />

  <loginForm />
  <myTable />
-->

<bootStrapTable />


</div>
</template>

<script>
import user from './User.vue'
import myTable from './MyTable.vue'
import loginForm from './LoginForm.vue'
import bootStrapTable from './BootstrapTable.vue'

export default {
  components: {
    'my-user': user,
    myTable,
    loginForm,
    bootStrapTable,
  },
  data () {
    return {
      message: 'Hello',
      users: [
        {name: 'Alex', description: 'This is our admin', isActive: true},
        {name: 'Jack', description: 'This is our manager', isActive: false},
        {name: 'John', description: 'This is our client', isActive: false},
      ]
    }
  },
  methods: {
    onLogin (data) {
      console.log('child component said login', data)
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

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
