<script>
export default {
    name : "AppMain"
}
</script>

<template>
    <div id="new_content_wrapper" class="d-flex justify-content-between align-items-center">
        <div class="nav_left">
            <h2 class>CONTENT GOES HERE</h2>
        </div>
        <div class="nav_right">                  
        </div>            
    </div>
    <div id="main_link_wrapper" class="container">
        <ul class="d-flex justify-content-around list-unstyled">
            <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
            <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
            <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
            <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
            <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>

        </ul>        


    </div>
</template>


<style scoped>
  #new_content_wrapper{
    color: white;
    background-color: black;
    max-width: 1400px;
    margin: auto;
    min-height: 80px;
}

#main_link_wrapper{
    color: white;
    background-color: rgb(58, 19, 166);
    max-width: 1400px;
    margin: auto;
    min-height: 80px;
}
.main_img_list{ 
    height: 70px;
    padding: 0.2rem;
}


</style>