<script>
export default {
    name: "AppMain",
    props: ["images"],
}
</script>

<template>
    <div id="new_content_wrapper">  
        <div class="container p-2">        
            <h5>CONTENT GOES HERE</h5>
        </div>           
    </div>  
    <div id="main_link_wrapper"> 
        <div class="container" >
            <ul class="d-flex justify-content-around list-unstyled">
                <div v-for="image in images">
                    <a class="p-1" href="#">
                        <li class="d-flex align-items-center">
                            <img class="main_img_list" :src="image.path" alt="">
                            <p class="icon_title">{{image.name.toUpperCase()}}</p>
                        </li>
                    </a>                    
                </div>
            </ul>    
        </div>
    </div>
    
</template>


<style scoped>
  #new_content_wrapper{
    color: white;
    background-color: rgb(28, 28, 28);
    margin: auto;
    height: 15vh;
}
/******************************** */
#main_link_wrapper{
    color: white;
    background-color: rgb(2, 130, 249);
    margin: auto;
    height: 15vh;
    }
.main_img_list{ 
    height: 50px;
    padding: 0.2rem;
}
.icon_title{
    color: white;
    font-size: 0.7rem;
    padding-left: 0.5rem;
    margin: 0;
}


/***********JUMBO********************* */



</style>