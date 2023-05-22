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
                <div class="left_column m-2 p-1">
                    <h6>DC COMICS</h6>
                    <ul class="list-unstyled">
                        <a v-show="link != 'Collectibles'&& link != 'Fans' && link != 'Shop'" :key="link" v-for="link in links" href="#"><li><small>{{link}}</small></li></a>
                      
                    </ul>
                    <h6>SHOP</h6>
                    <ul class="list-unstyled">
                        <a href="#"><li><small>Shop DC</small></li></a>
                        <a href="#"><li><small>Shop DC Collectibles</small></li></a>
                       
                    </ul>
                </div>
                <div class="center_column m-2 p-1">
                    <h6>DC</h6>
                    <ul class="list-unstyled">
                        <a href="#"><li><small>Terms Of Use</small></li></a>
                        <a href="#"><li><small>Privacy policy (New)</small></li></a>
                        <a href="#"><li><small>Ad Choises</small></li></a>
                        <a href="#"><li><small>Advertising</small></li></a>
                        <a href="#"><li><small>Jobs</small></li></a>
                        <a href="#"><li><small>Subscriptions</small></li></a>
                        <a href="#"><li><small>Talent Workshops</small></li></a>
                        <a href="#"><li><small>CPSC Certificates</small></li></a>
                        <a href="#"><li><small>Ratings</small></li></a>
                        <a href="#"><li><small>Shop Help</small></li></a>
                        <a href="#"><li><small>Contacts Us</small></li></a>                         
                    </ul>

                </div>
                <div class="right_column m-2 p-1">
                    <h6>SITES</h6>
                    <ul class="list-unstyled">
                        <a href="#"><li><small>DC</small></li></a>
                        <a href="#"><li><small>MAD Magazine</small></li></a>
                        <a href="#"><li><small>DC Kids</small></li></a>
                        <a href="#"><li><small>DC Universe</small></li></a>
                        <a href="#"><li><small>DC Power Visa</small></li></a>                       
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
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-twitter.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-youtube.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-pinterest.png" alt=""></li></a>
                    <a class="p-2" href="#"><li><img src="../assets/img/footer-periscope.png" alt=""></li></a>

                </ul>
            </div>
        
        </div>
    </div>    
</template>  

<style scoped lang="scss">

#jumbo{      
    margin: auto;
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);

}

#jumbo_wrapper{
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
    padding: 1rem 0;
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
}


#nav_logo{
    height: 60px;
    padding: 0.5rem;
}

img{
    height: 30px;
}
</style>