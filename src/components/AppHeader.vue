<script>
export default {
    name: "AppHeader"
}
</script>

<template>
        <div id="nav_wrapper" class="d-flex justify-content-between align-items-center">
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

</template>

<style scoped>


#nav_wrapper{
    background-color: white;
    max-width: 1400px;
    margin: auto;
    min-height: 80px;
}


#nav_logo{
    height: 60px;
    padding: 0.5rem;
}
</style>