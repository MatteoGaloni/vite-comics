<script>
import json from '../assets/json/dc-comics.json';

export default {
    name: "Slider",
    props: {
        thumbs: Object,
    },
    data() {
        return {
            myJson: json
        }
    }
}
</script>

<template>
    <div id="slider_wrapper">
        <button id="current_btn" class="btn btn-primary border-primary text-white">CURRENT SERIES</button>
        <div class="container p-2 d-flex flex-wrap">
            <div v-for="thumb in myJson" class="slide p-2">
                <img :src="thumb.thumb" alt="icon">
                <h6 class="slide_title p-2">{{ thumb.series }}</h6>
                <span class="slide_title pl-2">{{ thumb.price }}</span>
            </div>
            <button id="load_btn" class="btn btn-primary border-primary text-white">LOAD MORE</button>
        </div>
    </div>
</template>

<style scoped lang="scss">
#slider_wrapper {
    color: white;
    background-color: rgb(28, 28, 28);
    margin: auto;
    padding-top: 3rem;
}



.slide {
    width: calc(100% / 6);

    &:hover {
        opacity: 0.7;
        cursor: pointer;
    }

    img {
        width: 100%;
        height: 171px;
        object-fit: cover;
        object-position: top;

    }

    .slide_title {
        color: darkgray;
    }
}

#current_btn {
    position: absolute;
    left: 12%;
    top: 55%;
    padding: 0.5rem 1rem;
}

#load_btn {
    margin: 0 auto 1rem;
}
</style>