<template>
  <div>
    <div class="conteiner">
      <table class="tabela-painel">
        <thead class="tabela__Cabecalho">
          <th id class="cabecalho c1">Cursos</th>
          <th class="cabecalho" colspan="2">Ações</th>
        </thead>
        <tbody>
          <tr class="row">
            <td class="dadoTabela-curso c1">Investimento Para iniciantes</td>
            <td class="dadoTabela-botton">
              <button class="botton-editar">Editar</button>
            </td>
            <td class="dadoTabela-botton">
              <button class="botton-excluir">Excluir</button>
            </td>
          </tr>
          <tr class="row">
            <td class="dadoTabela-curso c1">Poupando e Rendendo</td>
            <td class="dadoTabela-botton c2">
              <button class="botton-editar">Editar</button>
            </td>
            <td class="dadoTabela-botton c3">
              <button class="botton-excluir">Excluir</button>
            </td>
          </tr>
          <tr class="row">
            <td class="dadoTabela-curso c1">Independência Financeira</td>
            <td class="dadoTabela-botton c2">
              <button class="botton-editar">Editar</button>
            </td>
            <td class="dadoTabela-botton c3">
              <button class="botton-excluir">Excluir</button>
            </td>
          </tr>
        </tbody>
      </table>
    <button id="button-novo">Criar um novo curso</button>
    </div>
  </div>
</template>
<script>
export default {
  nome: "PainelAcoes",

};
</script>
<style scoped>
.conteiner {
display: flex;
justify-content: space-around;
align-items: center;
flex-wrap: wrap

}
.tabela-painel {
  margin-top: 107px;
  /*margin-left: 82px;*/
  width: 812px;
  flex-wrap: wrap;
  border: 1px solid #EBEBEB;
  border-collapse: collapse;

  /*
  position: absolute;
  width: 63px;
  height: 28px;
  left: 106px;
  top: 405px;
  */
}
#button-novo{
  font-size: 20px;
  font-weight: 400;
  background-color: #419488;
  border-radius: 62px;
  color: #ffffff;
  margin-top: 53px;
  width: 233px;
  height: 51px;
  cursor: pointer;

}
.tabela__Cabecalho {
  background-color: #ebebeb;
}
.cabecalho {
  color: #000000;
  font-size: 24px;
  font-style: normal;
  font-family: Ubuntu;
  text-align: left;
}
.c1 {
  max-width: 100px;
}
button:hover {
  background: #ebebeb;
  border: solid 1px;
  cursor: pointer;
}
.botton-editar {
  background-color: #f8c23a;
  width: 87px;
  height: 22px;
  font-family: Ubuntu;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 17px;
  margin-bottom: 11px;
  margin-top: 11px;
}

.botton-excluir {
  background-color: #f8513a;
  width: 87px;
  height: 22px;
  font-family: Ubuntu;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 17px;
  margin-bottom: 11px;
  margin-top: 11px;
}
.dadoTabela-botton {
  text-align: left;
  margin: 12px;
  width: 20px;
  
}

@media screen and (max-width: 480px) {

  .tabela-painel{
    margin: 20px;
  }
  #button-novo{
    margin-bottom: 53px;
  }
}
@media (max-width:1045px) {
  .tabela-painel{
    margin: 20px;
  }
  #button-novo{
    margin-bottom: 53px;
  }
}
=======
  }
}
@media (max-width:1045px) {
  .tabela-painel{
    margin: 20px;
  }
  #button-novo{
    margin-bottom: 53px;
  }
}

</style>
