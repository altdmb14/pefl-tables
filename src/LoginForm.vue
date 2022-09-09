<template>
<div>

<h3>Login form</h3>
<div>
    <div>
    <label>Email:</label>
    <input type='text' v-model='email' />
    </div>

    <div>
    <label>Password:</label>
    <input type='password' v-model='password' />
    </div>

    <div>
    <button @click='login'>Login</button>
    </div>
</div>

</div>
</template>

<script>
export default {
    data () {
        return {
            email: '',
            password: ''
        }
    },
    methods: {
        login () {
           console.log('login', this.email, this.password)
        }
    }
}
</script>