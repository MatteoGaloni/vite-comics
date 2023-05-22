<script>
export default {
    name: "AppMain",
    props: ["images"],
}
</script>

<template> 
    <div id="main_link_wrapper"> 
        <div class="container" >
            <ul class="d-flex justify-content-around m-0">
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


<style scoped lang="scss">

/******************************** */
#main_link_wrapper{
    color: white;
    background-color: rgb(2, 130, 249);
    margin: auto;
    padding: 1rem;
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