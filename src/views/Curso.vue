<template>
  <div>
    <div class="container">
      <div class="curso">
        <div class="conteudo">
          <h1>{{listCursos.CursoTitulo}}</h1>
          <p>{{listCursos.CursoDescricao}}</p>
        </div>
        <div class="image">
          <img src="../assets/images/image3.png" alt="">
        </div>
      </div>
      <div>
      <div class="aula">
        <div class="video">
          <iframe width="462" height="261" :src="AulaUmLink" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
        <div>
          <h2>{{listCursos.AulaUmTitulo}}</h2>
          <p>{{listCursos.DescricaoAulaUm}}</p>
        </div>
      </div>
      <hr>
      </div>
  </div>
  </div>
</template>

<script>
import { mapActions, mapGetters } from 'vuex'
export default {
  mounted(){
    this.getCursos()
  },
  methods: {
    ...mapActions('getCurso',['getCursos'])
  },
  computed: {
    ...mapGetters('getCurso',['listCursos'])
  },
}
</script>

<style scoped>

  .curso {
    display: flex;
  }

  h1 {
    max-width: 450px;
    font-size: 55px;
    font-weight: 700;
    color: #FF4081;
    margin: 94px 0 22px 202px;
  }

  .conteudo p {
    max-width: 461px;
    font-size: 20px;
    font-weight: 300;
    margin-left: 202px;
  }

  .image img {
    margin: 81px 0 81px 88px;
    padding-right: 35px;
  }

  .aula {
    display: flex;
    background-color: #F6F6F6;
  }

  .aula p {
    max-width: 501px;
    margin-left: 76px;
    font-size: 20px;
    font-weight: 300;
    padding-right: 35px;
  }

  iframe {
    margin: 75px 76px 73px 213px
  }

  h2 {
    font-size: 35px;
    font-weight: 700;
    color: #FF4081;
    margin: 75px 0 26px 76px;
  }

  hr {
    margin: 0 auto;
    max-width: 1244px;
    width: 100%;
    height: 3px;
    background-color: #C4C4C4;
  }

  @media screen and (max-width: 1075px){
    h1, .conteudo p, iframe {
      margin-left: 10px;
    } 
    .image img, .aula p, h2 {
      margin-left: 25px;
    }
    iframe {
      margin-right: 10px;
    }
  }
  @media screen and (max-width: 800px){
    .curso, .aula {
      flex-wrap: wrap;
      justify-content: center;
      text-align: center;
    }
    h1, .aula p, .conteudo p {
      max-width: 500px;
    }
    hr {
      margin-top: 15px;
    }
    h2 {
      margin-top: 5px;
    }
    .image img {  
      width: 100%;
    }
    iframe {
      width: 100%;
      margin-left: 0;
    }
  }
  @media screen and (max-width: 500px){
    .image img { 
      max-width: 300px;
    }
    iframe {
      width: 280px;
      height: auto;
    }
  }



</style>