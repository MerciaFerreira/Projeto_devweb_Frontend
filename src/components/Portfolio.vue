<template>
    <section class="bg-light" id="portfolio">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center">
            <h2 class="section-heading text-uppercase">Livros</h2>
            <h3 class="section-subheading text-muted">Gêneros literários.</h3>
          </div>
        </div>
        <div class="row">
          
            <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj, key) in portfolioJSON" :key="key">
                <a class="portfolio-link" data-toggle="modal" href="#portfolioModal2">
                    <div class="portfolio-hover">
                        <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                        </div>
                    </div>
                    <img class="img-fluid" src="img/portfolio/02-thumbnail.jpg" alt="">
                </a>
                <div class="portfolio-caption">
                    <h4>{{ obj.caption }}</h4>
                    <p class="text-muted">{{ obj.title }}</p>
                </div>
            </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data: () => ({
        portfolioJSON: [
            {
                img: '/something/random/img.jpg',
                caption: 'Suspense',
                title: 'Livros de suspense'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Romance',
                title: 'Livros de Romance'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Comédia',
                title: 'Livros de Comédia'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Terror',
                title: 'Livros de Terror'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Aventura',
                title: 'Livros de Aventura'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Ficção',
                title: 'Livros de Ficção' 
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Ação',
                title: 'Livros de Ação'
            }
        ]
    })
}
</script>

<style lang="css">

</style>


