<template>
    <div class="container" v-bind:key="cadastro.id" v-for="cadastro in cadastros">
        <p>
            ID:{{cadastro.id}}
        </p>
        <br> 
        <p>
            Descrição:{{cadastro.descrição}}
        </p>
        <p v-if="cadastro.estaCompleta" id="completo">
            Cadastro está concluido!!
        </p>
        <p v-else id ="inCompleto">
            Erro:Cadastro Incompleto.. Tente novamente!!
        </p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            cadastros:[
            {id: 1, descricao: "Descrição 111111", estaCompleta: true},
            {id: 2, descricao: "Descrição 222222", estaCompleta: false},
            {id: 3, descricao: "Descrição 333333", estaCompleta: false},
            {id: 4, descricao: "Descrição 4444444", estaCompleta: true},
            {id: 5, descricao: "Descrição 5555555", estaCompleta: true},
            {id: 6, descricao: "Descrição 666666", estaCompleta: false}
            ]
        }
    },
}
</script>

<style scoped>
.container{
  display: flex;
  justify-content: center;
  width: 90%;
  flex-wrap: wrap;
  width: 300px;
  height: 250px;
  text-align: center;
}
#completo{
  color: green;
  font-weight: bolder;
  font-size: 1.1em;
  text-align: center;
}
#inCompleto{
  color: orange;
  font-weight: bolder;
  font-size: 1.1em;
  text-align: center;
}
p{
    text-align: center;
    
}
</style>