<template>
  <div id="wrapper">
    <Header />

    <section class="section lb text-muted">
      <div class="container">
        <div class="row grid-style">
          <div class="col-lg-3 col-md-6 col-sm-12 col-xs-12" v-for="listRecipe in listRecipes">
            <Recipe
              :judul="listRecipe.title"
              :gambar="listRecipe.thumb"
              :level="listRecipe.dificulty"
              :porsi="listRecipe.portion"
              :waktu="listRecipe.times"
            />
          </div><!-- end col -->
        </div><!-- end row -->
        
        <hr class="invis">

          <div class="row">
            <div class="col-md-12 text-center">
              <nav aria-label="Page navigation">
                <ul class="pagination justify-content-center">
                  <li class="page-item"><a class="page-link" href="#">1</a></li>
                  <li class="page-item"><a class="page-link" href="#">2</a></li>
                  <li class="page-item"><a class="page-link" href="#">3</a></li>
                  <li class="page-item">
                    <a class="page-link" href="#">Next</a>
                  </li>
                </ul>
              </nav>
            </div><!-- end col -->
        </div> <!-- end row -->
        
      </div> <!-- end container -->
    </section><!-- end album -->

    <Footer />  

    <!-- <div class="dmtop">Scroll to Top</div> -->
        
  </div><!-- end wrapper -->
</template>

<script>
// import Header, Recipe, Footer
import Header from './components/Header.vue';
import Recipe from './components/Recipe.vue';
import Footer from './components/Footer.vue';

export default {
  name: "App",
  components: {
    Header,
    Recipe,
    Footer,
  },
  data(){
      return{
          listRecipes: []
      }
  },
  mounted() {
      fetch("https://masak-apa-tomorisakura.vercel.app/api/recipes/")
      .then(response => response.json())
      .then(response => {
          this.listRecipes = response.results
          // console.log(response.results)
      })
  }
}
</script>


<style>
</style>
