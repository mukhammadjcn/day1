<template>
    <div class="testimons">
        <div class="container">
            <div class="testimons__img">
                <img src="../assets/images/img5.png" alt="">
            </div>
            <div class="testimons__info">
                <h3 class="label">Testimonials</h3>
                <h2 class="title">Reviews</h2>
                <div class="feedback">
                    <p class="info">"The sky was cloudless and of a deep dark blue the spectacle before us was indeed sublime sky was cloudless and of a deep dark."</p>
                    <h2 class="miniTitle">Jaroslav Brabec</h2>
                    <p class="miniInfo">Microsoft</p>
                    <svg width="48" height="36" viewBox="0 0 48 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M20 0C7.784 2.412 0 13.168 0 23.45C0 31.39 5.572 36 11.602 36C16.832 36 22 32.406 22 26.042C22 20.838 18.19 16.528 13.208 15.744C13.642 11.736 17.538 5.922 21.968 4.252L20 0ZM46 0C33.784 2.412 26 13.168 26 23.45C26 31.39 31.572 36 37.602 36C42.832 36 48 32.406 48 26.042C48 20.838 44.19 16.528 39.208 15.744C39.642 11.736 43.538 5.922 47.968 4.252L46 0Z" fill="#4DB282"/>
                    </svg>
                </div>
                <div class="row">
                    <svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="48" height="48" rx="24" fill="#F07566"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M16.3258 23.2196L25.4156 14.3195C25.6258 14.1135 25.9065 14 26.2057 14C26.5049 14 26.7856 14.1135 26.9958 14.3195L27.6652 14.9748C28.1008 15.4018 28.1008 16.0958 27.6652 16.5221L20.0323 23.9959L27.6737 31.4779C27.8839 31.6839 28 31.9586 28 32.2514C28 32.5446 27.8839 32.8192 27.6737 33.0254L27.0043 33.6805C26.7939 33.8865 26.5134 34 26.2142 34C25.9149 34 25.6343 33.8865 25.424 33.6805L16.3258 24.7723C16.1151 24.5656 15.9993 24.2897 16 23.9963C15.9993 23.7019 16.1151 23.4261 16.3258 23.2196Z" fill="white"/>
                    </svg>
                    <svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <rect width="48" height="48" rx="24" fill="#F07566"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M31.6742 23.2196L22.5844 14.3195C22.3742 14.1135 22.0935 14 21.7943 14C21.4951 14 21.2144 14.1135 21.0042 14.3195L20.3348 14.9748C19.8992 15.4018 19.8992 16.0958 20.3348 16.5221L27.9677 23.9959L20.3263 31.4779C20.1161 31.6839 20 31.9586 20 32.2514C20 32.5446 20.1161 32.8192 20.3263 33.0254L20.9957 33.6805C21.2061 33.8865 21.4866 34 21.7858 34C22.0851 34 22.3657 33.8865 22.576 33.6805L31.6742 24.7723C31.8849 24.5656 32.0007 24.2897 32 23.9963C32.0007 23.7019 31.8849 23.4261 31.6742 23.2196Z" fill="white"/>
                    </svg>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name : "Testimons"
}
</script>

<style lang="scss">
.testimons{
    padding: 64px 0;
    .container{
        display: flex;
        align-items: center;
        gap: 120px;
    }
    .feedback{
        position: relative;
        margin: 36px 0;
        padding: 28px 32px;
        background: #FFFFFF;
        box-shadow: 0px 24px 48px rgba(0, 17, 86, 0.0799083);
        border-radius: 8px;
        .miniTitle{
            margin: 14px 0 6px;
        }
        svg{
            position: absolute;
            top: 0;
            right: 0;
            transform: translate(-50%, -50%);
        }
    }
    &__info{
        flex-basis: 50%;
        .row{
            display: flex;
            align-items: center;
            gap: 16px;
        }
        .title{
            margin-top: 18px;
        }
    }
    &__img{
        img{
            width: 100%;
        }
    }
}

@media(max-width:776px){
    .testimons{
        .container{
            flex-direction: column;
        }
        &__info{
            display: flex;
            flex-direction: column;
            align-items: center;
        }
    }
}
</style>