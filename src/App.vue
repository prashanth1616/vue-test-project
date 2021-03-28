<template>
<div id="App">
@{{user.username}} - {{fullname}}

</div>
</template>

<script>


export default {
  name: 'App',
  data(){
    return {
      follower:0,
      user:{
        id:1,
        firstname:"Prashanth",
        lastname:"Reddy",
        email:"prashanth@live.com",
        username:"_chinnared",
        isadmin:true
    }
}
},
 computed:{
   fullname(){
return `${this.user.firstname} ${this.user.lastname}`
 }
 }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
