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
</template>

<style scoped lang="scss">


#nav_wrapper{
    background-color: white;
    margin: auto;
    height: 15vh;
}

#nav_logo{
    height: 65px;
}

.link{
    color: black;
}
/* 
.link::after{
    border: red 1px;
} */


</style>