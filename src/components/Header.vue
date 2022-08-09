<template>
  <section id="cta" class="jumbotron text-center">
    <div class="container">
      <a href="food-index.html"><img src="/src/assets/images/version/food-logo.png" alt="" class="img-fluid"></a>
      <p>Setiap tahun kami menyelenggarakan Penghargaan Blog Makanan Terbaik, kami kagum dengan kedalaman, variasi, kreativitas, dan kecerdasan dari blog makanan yang dinominasikan</p>
      <a href="#" class="btn btn-primary">Daftar Resep</a>
    </div>
  </section>

  <header class="header">
    <div class="container">
      <nav class="navbar navbar-inverse navbar-toggleable-md">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#RecipeListmenu" aria-controls="RecipeListmenu" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-md-center" id="RecipeListmenu">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link" href="food-index.html">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="food-category.html">Kategori Resep</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="food-contact.html">Hubungi Kami</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#"><i class="fa fa-play-circle-o"></i> Youtube Channel</a>
            </li>  
          </ul>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
  export default {
    name: "Header",
  }
</script>

<style>
</style>