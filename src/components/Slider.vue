<script>
export default {
    name: "Slider",
    props: {
       thumbs : Object,
    }
}
</script>

<template>
        <div id="slider_wrapper">  
            <div class="container p-2 d-flex flex-wrap">        
                <div v-for="thumb in thumbs" class="slide p-2">
                    <img :src="thumb.thumb" alt="icon">
                    <h6 class="slide_title">{{ thumb.series }}</h6>
                </div>


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
    img{
    width: 100%;
    height: 171px;
    object-fit: cover;
    object-position: top;
        &:hover {
        opacity: 0.7;
        cursor: pointer;
        } 
    }
}

</style>