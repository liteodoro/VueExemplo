<template>
  <table class="table">

    <tr>

      <th>Nome</th>

      <th>Desescricao</th>

      <th>Quant</th>

      <th>Valor</th>

      <th>//</th>

      <th>X</th>

    </tr>

    <tr v-for="produto in produtos" :key="produto.id">

      <td>{{ produto.nome }}</td>

      <td>{{ produto.descricao }}</td>

      <td>{{ produto.quant }}</td>

      <td>R$ {{ produtos.valor.tofixed }}</td>

      <td @click="getProduto(produto)">//</td>

      <td @click="deleteProduto(Produto)">X</td>

    </tr>

  </table>
</template>

<script>
import Produto from "./Produto";
let produto = new Produto();

export default {
   name:"ProdutoListcomponent",
   data(){
       return{
           produtos: produto.getAll(),
           produto,
       };
   },
  methods: {
    getProduto(produto) {
      console.log(produto);
      this.produto = produto;
    },
  },
};
</script>

<style>

</style>