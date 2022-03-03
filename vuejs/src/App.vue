<template>
<div>
  <div class="app-header">
    <Navbar />
  </div>
  
  <div class="app-container">
    <router-view />
  </div>
</div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Sidebar from "@/components/Sidebar.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Sidebar
  },
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: 'poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
  height: 100vh;
}

.app-header{
  width: 100%;
  height: 55px;
}

.app-container{
  display: flex;
  width: 100%;
  height: calc(100vh - 55px);
}

a{
  text-decoration: none;
  color: #5a5a5a;
}

img{
  cursor: pointer;
}

.div-flex{
  display: flex;
  align-items: center;
}
</style>
