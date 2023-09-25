<template>
  <Login/>
</template>
<script>
//import GetData from "../utils/api.js";
import Login from './pages/Login.vue'
export default {
  name: "App",
  data() {
    return {
      username: "",
      password: "",
    };
  },
  methods: {
    async login() {
      if (this.username && this.password) {
        console.log(this.username, this.password);
        alert(this.username, this.password);
        return;
      }
      alert("Vui long nhap tai khoan va mat khau");
    },
  },
  components : {
    Login
  }
};
</script>