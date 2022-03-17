<template>
  <div class="teste-for">
      <h2>Teste For</h2>
      <ol class="lista-contatos">
          <li v-for="info of infos" v-bind:key="info.id">
              <p> {{info.nome}},  {{info.telefone}}</p>
          </li>
      </ol>
  </div>
</template>

<script>
export default {
    name: 'TesteFor',
    data(){
        return{
            infos: [
                {id: 1,
                nome: "Lucas",
                telefone: 984907163},
                {id: 2, 
                nome: 'João', 
                telefone: 984477559},
            ]
        }
    }
}
</script>

<style scoped>
    
    
</style>