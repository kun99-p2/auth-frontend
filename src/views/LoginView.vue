<template>
  <div class="id">
    <h1>Login</h1>
    <form>
      <label for="fname">Username:</label><br>
      <input type="text" id="uname" name="uname"><br>
      <label for="lname">Password:</label><br>
      <input type="password" id="passw" name="passw"><br><br>
    </form>
  </div>
  <div class="submit">
    <button @click="cancel" style="margin-right: 10px;">
    Cancel
    </button>
    <button @click="register">
      Login
    </button>
  </div>
</template>
  
<style>
</style>

<script>
export default {
  methods: {
    login() {
      //authentication in backend
    },
    cancel() {
      this.$router.push('/');
    }
  }
};
</script>
  