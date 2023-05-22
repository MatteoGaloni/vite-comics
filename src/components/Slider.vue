<script>
export default {
    name : "Slider",
}
</script>

<template>
        <div id="slider_wrapper">  
            <div class="container p-2 d-flex flex-wrap">        
                <div class="slide">1</div>
                <div class="slide">2</div>
                <div class="slide">3</div>
                <div class="slide">4</div>
                <div class="slide">5</div>
                <div class="slide">6</div>
                <div class="slide">1</div>
                <div class="slide">2</div>
                <div class="slide">3</div>
                <div class="slide">4</div>
                <div class="slide">5</div>
                <div class="slide">6</div>
            </div>           
        </div> 
</template>

<style scoped lang="scss">
  #slider_wrapper{
    color: white;
    background-color: rgb(28, 28, 28);
    margin: auto;
}



.slide{
    width: calc(100% / 6);
}

</style>