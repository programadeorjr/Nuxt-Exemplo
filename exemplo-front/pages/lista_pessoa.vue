<template>
  <div class="container">
      <h1>{{titulo}}</h1>
  <ul>
      <li :key="item.id" v-for = "item in pessoas">
          <!-- Saída: Nome: Marcio -> 18 anos -->
      {{item.nome}} -> {{item.idade}}</li>
  </ul>
  <button>Clique aqui</button>
  </div>
</template>

<script>
export default {
    data: function (){
        return{
            titulo:"Lista de peassoas e idades",
            pessoas: [
                {id: 1,nome:"Pedro", idade:18},
                {id: 1,nome:"Maria", idade:13},
                {id: 1,nome:"Clara", idade:29},
                {id: 1,nome:"Ana", idade:17},
                {id: 1,nome:"Mayara", idade:23},
                {id: 1,nome:"Laura", idade:15},
            ]
        }
    }
}
</script>

<style>

</style>