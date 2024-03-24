<template>
   <div class="container">
    <div class="row">
      <div class="col-12 text-center">
        <h3>Ajouter une catégorie</h3>
      </div>
    </div>
    <div class="row">
      <div class="col-md-3"></div>
      <div class="col-md-6">
        <form>
          <div class="form-group">
            <label>Nom de la catégorie</label>
            <input type="text" class="form-control" v-model="categorieName" placeholder="Entrez le nom de la catégorie">
          </div>
          <div class="form-group">
            <label>Description de la catégorie</label>
            <textarea class="form-control" v-model="description" placeholder="Entrez la description de la catégorie"></textarea>
          </div>
          <div class="form-group">
            <label>Image de la catégorie</label>
            <input type="text" class="form-control" v-model="imageUrl" placeholder="Entrez l'URL de l'image de la catégorie">
          </div>
          <button type="button" class="btn btn-primary mb-2" @click="addCategory">Enregistrer</button>
        </form>
      </div>
      <div class="col-md-3"></div>
    </div>
  </div>
</template>
  
  <script>
  
  //const axios=require("axios");
  export default {
    data(){
   return {
     categorieName: "",
     description: "",
     imageUrl: "",
   }
    },
    methods:{
      addCategory(){
        console.log(this.categorieName,this.description)
  }
}};

  </script>
  <style scoped>

</style>