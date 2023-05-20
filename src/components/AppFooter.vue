<script>
export default {
    name: "AppFooter",
    props: ["links"],
}

</script>

<template>
    <div id="jumbo">
        <div id="jumbo_wrapper" class="container d-flex justify-content-between">
            <div class="link_left_container d-flex">
                <div class="left_column">
                    <h6>Titolo</h6>
                    <ul class="list-unstyled">
                        <a v-show="link != 'Collectibles'&& link != 'Fans' && link != 'Shop'" :key="link" v-for="link in links" href="#"><li><small>{{link}}</small></li></a>
                      
                    </ul>
                    <h6>Titolo</h6>
                    <ul class="list-unstyled">
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                       
                    </ul>
                </div>
                <div class="center_column">
                    <h6>Titolo</h6>
                    <ul class="list-unstyled">
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>                         
                    </ul>

                </div>
                <div class="center_column">
                    <h6>Titolo</h6>
                    <ul class="list-unstyled">
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>
                        <a href="#"><li><small>LINK</small></li></a>                       
                    </ul>

                </div>        
            </div>
        </div>
    </div>
    <div id="nav_wrapper" class="d-flex">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="nav_left">
               <button class="btn border-primary text-white">SIGN-UP NOW!</button>
            </div>
            <div class="nav_right">
                <ul class="d-flex list-unstyled align-items-center">
                    <a class="p-2" href="#"><li>FOLLOW US</li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-facebook.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-facebook.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-pinterest.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-pinterest.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-pinterest.png" alt=""></li></a>

                </ul>
            </div>
        
        </div>
    </div>    
</template>  

<style scoped>

#jumbo{      
    margin: auto;
    height: 45vh;
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);

}

#jumbo_wrapper{
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
    margin-bottom: 0;
}

small{
    color: grey;
}

#dc_big_logo{
    height: 200px;
}

#nav_wrapper{
    background-color:rgb(48, 48, 48);
    margin: auto;
    height: 10vh;
}


#nav_logo{
    height: 60px;
    padding: 0.5rem;
}
</style>