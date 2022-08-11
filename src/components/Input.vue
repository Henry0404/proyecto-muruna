<template>
  <div class="hello"> 
    <h1>{{ msg }}</h1>
      <input
      type="text"
      class="form-control my-2"
      placeholder="Ingresa Nombre"
      v-model="name"
    />
    <div class="form-group">
    <label class="text-left" for="exampleFormControlSelect1">Elige un nùmero</label>
    <select class="form-control" id="exampleFormControlSelect1" v-model="select">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
        <button
      class="btn btn-block mt-2 btn-dark"
      type="submit"
      v-on:click="procesar"
    >
      Procesar
    </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      name:'',
      select:'',
    }
  },
  methods:{
    procesar(){
      alert(`${this.name}, ${this.select}`)
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
