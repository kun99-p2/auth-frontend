<template>
  <div class="id">
    <h1>Registration</h1>
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
      Register
    </button>
  </div>
</template>
  
<style>
.id {
  font-size: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 25vh;
}
.submit {
  font-size: 20px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-left: 25px;
}
</style>

<script>
export default {
  methods: {
    register() {
      this.$router.push('/success');
    },
    cancel() {
      this.$router.push('/');
    }
  }
};
</script>
  