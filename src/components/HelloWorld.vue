<template>
  <div>
    <h2>Welcome to the Shop</h2>
    <h4>Your online grocery store</h4>
    <p>Sign Up for new user!!</p><span><router-link to="/signUp"><v-btn>Sign Up</v-btn></router-link></span>
    
  </div>
</template>

<script>

  export default {
    data() {
      return {
        
      }
    },
    methods: {
      
      }
      
    }
  
</script>

<style scoped>
  .button {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>
