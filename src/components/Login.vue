<template>
  <div class="login">
    <div class="login-box">
      <label for="username-input" type="text">Username </label>
      <input id="username-input" placeholder="A_Really_Cool_Name" />
      <label for="password-input" type="password">Password</label>
      <input id="password-input" placeholer="..." />
      <label for="show-password-checkbox"> Show password </label>
      <input id="show-password-checkbox" type="checkbox" />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String,
  },
})
export default class Login extends Vue {
  data() {
    return {
      username: "",
      password: "",
      loginError: "",
      loading: "",
    };
  }
  methods() {
    return {
      login: function () {},
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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
