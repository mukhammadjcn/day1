<template>
    <div class="team">
        <div class="container">
            <div class="team__label">
                <h2 class="label">Portfolio</h2>
                <h2 class="title">Company Cases</h2>
                <p class="info">Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle the same illusion which lifts the horizon of the sea.</p>
            </div>
            <div class="team__wrapper">
                <VueSlickCarousel v-bind="settings">
                    <div class="team__user">
                        <img src="https://picsum.photos/400/400" alt="">
                        <h3 class="miniTitle">Ingo Schimpff</h3>
                        <p class="info">Manager</p>
                    </div>
                    <div class="team__user">
                        <img src="https://picsum.photos/400/401" alt="">
                        <h3 class="miniTitle">Ingo Schimpff</h3>
                        <p class="info">Director</p>
                    </div>
                    <div class="team__user">
                        <img src="https://picsum.photos/400/402" alt="">
                        <h3 class="miniTitle">Ingo Schimpff</h3>
                        <p class="info">Manager</p>
                    </div>
                    <div class="team__user">
                        <img src="https://picsum.photos/400/403" alt="">
                        <h3 class="miniTitle">Ingo Schimpff</h3>
                        <p class="info">Director</p>
                    </div>
                </VueSlickCarousel>
            </div>
        </div>
    </div>
</template>

<script>

import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    name : "Team",
    components: { VueSlickCarousel },
    data(){
        return{
            settings : {
                "dots": true,
                "infinite": true,
                "speed": 500,
                "slidesToShow": 3,
                "slidesToScroll": 1,
                "initialSlide": 0,
                "autoplay" : true,
                "responsive": [
                    {
                    "breakpoint": 1024,
                    "settings": {
                        "slidesToShow": 3,
                        "slidesToScroll": 3,
                        "infinite": true,
                        "dots": true
                    }
                    },
                    {
                    "breakpoint": 800,
                    "settings": {
                        "slidesToShow": 2,
                        "slidesToScroll": 2,
                        "initialSlide": 2
                    }
                    },
                    {
                    "breakpoint": 500,
                    "settings": {
                        "slidesToShow": 1,
                        "slidesToScroll": 1
                    }
                    }
                ]
                }
        }
    }
}
</script>

<style lang="scss">
.team{
    padding: 120px 0;
    &__label{
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 80%;
        margin: auto;
        .info{
            text-align: center;
        }
        .title{
            margin: 20px 0 20px;
        }
    }
    &__user{
        padding: 16px;
        border-radius: 8px;
        background: #FFFFFF;
        border: 1px solid #E6EDF5;
        transition: 0.1s ease-in;
        img{
            border-radius: 8px 8px 50px 8px;
            width: 100%;
            object-fit: cover;
        }
        &:hover{
            background: #FFFFFF;
            box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
            border-color: transparent;
            transform: scale(1.01);
        }
        .miniTitle{
            margin: 24px 0 16px;
        }
    }
    &__wrapper{
        padding: 64px 0 36px;
        .slick-slide{
            padding: 0 8px;
        }
        .slick-dots li button:before{
            font-size: 8px;
            opacity: 1;
            color: #FFE4E1;
        }
        .slick-dots li.slick-active button:before{
            font-size: 14px;
            color: #F07566;
        }
        .slick-dots{
            bottom: -48px;
        }
    }
}
</style>