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
                <img id="nav_logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/DC_Comics_logo.svg/1200px-DC_Comics_logo.svg.png" alt="">
            </div>
            <div class="nav_right">
                <ul class="d-flex list-unstyled">
                    <a :key="link" v-for="link in links" class="link p-1" href="#"><li>{{link}}</li></a>                
                </ul>
            </div>            
       </div>
    </div>
    <div id="jumbo">
        <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
</template>

<style scoped lang="scss">


#nav_wrapper{
    background-color: white;
}

.nav_left{
    padding: 1rem 0;
    #nav_logo{
    width: 65px;
    }
}

.nav_right{
    padding: 1rem 0;
}

.link{
    color: black;
    text-decoration: none;
    & :hover{
        opacity: 0.7;
    }
}

#jumbo{
    height: 310px;
    img{
        object-fit: cover;
        object-position: top;
        height: 100%;
        width: 100%;
    }
}
</style>