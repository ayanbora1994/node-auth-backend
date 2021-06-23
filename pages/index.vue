<template>
  <div>
    <div v-if="$auth.loggedIn">
      Logged In
      {{ $auth.user.email }}
    </div>
    <div v-else>
      <router-link to="/login">LOGIN</router-link>
    </div>
  </div>
</template>