<template>
  <div class="hello">
    <h1>{{msg}}</h1>
    <div>
      <h1>{{name}}</h1>
      <input type="text" placeholder="your email" v-model="email"> <br><br>
         <input type="text" placeholder="your password"  v-model="name"><br><br>
      <button v-on:click="getData(zain)" type="button">click me</button> <br><br>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },data() { 
    return {
      email: null,
      password: null,

    }
  },
  methods:{
    getData(){
      console.warn("value : ",this.email,this.password)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
