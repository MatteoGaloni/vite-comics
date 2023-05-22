<script>
export default {
    name: "AppHeader",
    props: {
        links: Object,
    }
}
</script>

<template>
    <div id="nav_wrapper" class="d-flex">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="nav_left">
                <img id="nav_logo"
                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/DC_Comics_logo.svg/1200px-DC_Comics_logo.svg.png"
                    alt="">
            </div>
            <div class="nav_right">
                <ul class="d-flex list-unstyled">
                    <a :key="link" v-for="link in links" class="link p-1" href="#">
                        <li>{{ link }}</li>
                    </a>
                </ul>
            </div>
        </div>
    </div>
    <div id="jumbo">
        <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img class="carousel_img d-block w-100" src="../assets/img/jumbotron.jpg" alt="First slide">
                </div>
                <div class="carousel-item">
                    <img class="carousel_img d-block w-100"
                        src="https://www.hollywoodreporter.com/wp-content/uploads/2015/05/gallerychar_1900x900_justiceleague_52ab8e54d0a6f0.42170553.jpg?w=3000"
                        alt="Second slide">
                </div>
                <div class="carousel-item">
                    <img class="carousel_img d-block w-100"
                        src="https://hips.hearstapps.com/hmg-prod/images/dc-movies-in-order-05-justice-league-1608143609.jpg"
                        alt="Third slide">
                </div>
            </div>
            <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </div>
</template>

<style scoped lang="scss">
#nav_wrapper {
    background-color: white;
}

.nav_left {
    padding: 1rem 0;

    #nav_logo {
        width: 65px;
    }
}

.nav_right {
    padding: 1rem 0;
}

.link {
    color: black;
    text-decoration: none;

    & :hover {
        opacity: 0.7;
    }
}

#jumbo {
    height: 310px;

}

.carousel_img {
    object-fit: cover;
    object-position: top;
    height: 310px;
    width: 100%;
}
</style>