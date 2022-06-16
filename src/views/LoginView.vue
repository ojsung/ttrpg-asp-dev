<template>
  <div class="login">
    <Login />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Login from "@/components/Login.vue"; // @ is an alias to /src

@Options({
  components: {
    Login,
  },
})
export default class LoginView extends Vue {}
</script>
