<script>
export default {
    name: "AppHeader"
}
</script>

<template>
    <div id="nav_wrapper">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="nav_left">
                <img id="nav_logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/DC_Comics_logo.svg/1200px-DC_Comics_logo.svg.png" alt="">
            </div>
            <div class="nav_right">
                <ul class="d-flex list-unstyled">
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                    <a class="p-1" href="#"><li>LINK</li></a>
                </ul>
            </div>            
       </div>
    </div>
</template>

<style scoped>


#nav_wrapper{
    background-color: white;
    margin: auto;
    height: 15vh;
}


#nav_logo{
    height: 60px;
    padding: 0.5rem;
}
</style>