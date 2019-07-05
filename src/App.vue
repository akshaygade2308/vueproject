<template>
  <div id="app">
    <template>
            <v-toolbar dark color="primary">
                <v-toolbar-side-icon></v-toolbar-side-icon>

                <v-toolbar-title class="white--text">The Green Army</v-toolbar-title>

                <v-spacer></v-spacer>

                <v-btn icon>
                <v-icon>search</v-icon>
                </v-btn>

                <!-- <v-btn icon>
                <v-icon>apps</v-icon>
                </v-btn>

                <v-btn icon>
                <v-icon>refresh</v-icon>
                </v-btn> -->

                <!-- <v-btn icon>
                <v-icon>more_vert</v-icon>
                </v-btn> -->
            </v-toolbar>
        </template>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/login">Login</router-link> 
      
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  data(){
    return{
      
        }
  } 
}
</script>



<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
