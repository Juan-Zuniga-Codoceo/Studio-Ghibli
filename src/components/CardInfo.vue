<template>
<div v-if="pelicula!=undefined">
    <div class="card text-start">
      <img class="card-img-top" style='height:300px;object-fit: contain' :src="pelicula.poster" alt="Title">
      <div class="card-body">
        <h4 class="card-title">Titulo original: {{pelicula.hepburn}}</h4>
        <h6 class="card-subtitle"><b>Titulo en inglés:</b> {{pelicula.title}}</h6>
        <p><b>Director:</b> {{pelicula.director}}<br>
           <b>Genero:</b> {{pelicula.genre}}<br>
           <b>Música:</b> {{pelicula.music}}<br>
           <b>Clasificación:</b> {{pelicula.rating}}<br>
           <b>Lanzamiento:</b> {{pelicula.release}}<br>
        </p>
        
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "card-comp",
  created() {},
  data() {
    return {};
  },
  props: {
    film:{
      type:Object,
      required:true
    }
  },
  computed:{
    pelicula(){
      if(this.film){
        return this.film.data
      }else{
        return{}
      }
    }
    
  },
  methods: {},
};
</script>

<style lang="scss" scoped></style>