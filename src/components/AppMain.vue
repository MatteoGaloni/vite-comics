<script>
export default {
    name : "AppMain"
}
</script>

<template>
    <div id="new_content_wrapper">
        <div class="container d-flex justify-content-between align-items-center">
            
            <div class="nav_left">
                <h2 class>CONTENT GOES HERE
                    <!-- <button @click="addbutton()">CLICCAMI</button> -->
                </h2>
            </div>
            <div class="nav_right">                  
            </div>            
        </div>
    </div>  
    <div id="main_link_wrapper"> 
        <div class="container" >
            <ul class="d-flex justify-content-around list-unstyled">
                <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
                <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
                <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
                <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
                <a class="p-1" href="#"><li><img class="main_img_list" src="../assets/img/buy-comics-digital-comics.png" alt=""></li></a>
            </ul>    
        </div>
    </div>
    
</template>


<style scoped>
  #new_content_wrapper{
    color: white;
    background-color: black;
    margin: auto;
    height: 15vh;
}
/******************************** */
#main_link_wrapper{
    color: white;
    background-color: rgb(58, 19, 166);
    margin: auto;
    height: 15vhpx;
    }
.main_img_list{ 
    height: 15vh;
    padding: 0.2rem;
}

ul{
    margin: 0;
}

/***********JUMBO********************* */



</style>