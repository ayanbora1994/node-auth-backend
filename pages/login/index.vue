<template>
    <div>
        Login Here
        <button @click="login">LOGIN</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            loginInfo: {
                email: "max@email.com",
                password: "gorilla123"
            }
        }
    },
    methods: {
        login() {
            this.$auth.loginWith('local', {
                data: this.loginInfo
            })
        }
    }
}
</script>