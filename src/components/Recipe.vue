<template>
    <div class="blog-box">
        <div class="post-media">
            <a href="food-single.html" :title="judul">
                <!-- .nonveg -->
                <span class="detail veg">Veg</span>
                <img :src="gambar" :alt="key" class="img-fluid">
                <div class="hovereffect"></div>
            </a>
        </div><!-- end media -->

        <div class="blog-meta big-meta">
            <div class="rating">
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
            </div>
            <h4><a href="food-single.html" :title="judul">{{ judul }}</a></h4>
            <p>Level: {{ level }}</p>
            <small><a href="#">{{ porsi }}</a></small>
            <small><a href="#">{{ waktu }}</a></small>
        </div><!-- end meta -->
    </div><!-- end blog-box -->
</template>

<script>
  export default {
    name: "Recipe",
    // props: ['judul']
    props: ["judul", "gambar", "key", "level", "porsi", "waktu"]
    // props: ["title", "thumb", "key", "dificulty", "portion", "times"]
  }
</script>

<style>
</style>