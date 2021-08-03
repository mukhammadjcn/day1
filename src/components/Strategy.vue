<template>
    <div class="strategy">
        <div class="container">
            <div class="strategy__img">
                <img src="../assets/images/strBg.png" alt="">
                <svg width="128" height="128" viewBox="0 0 128 128" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect width="128" height="128" rx="8" fill="#FBD34B"/>
                    <path d="M83 64L53 83V45L83 64Z" fill="white"/>
                </svg>
            </div>
            <div class="strategy__info">
                <h2 class="title">Strategy, technology and design</h2>
                <p class="info">Apparently we had reached a great height in the atmosphere, for the sky was a dead black.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : "Strategy"
}
</script>

<style lang="scss">
.strategy{
    padding: 86px 0;
    background-color: #F07566;
    .container{
        display: flex;
        align-items: center;
        gap: 164px;
    }
    &__img{
        height: 240px;
        flex-basis: 40%;
        position: relative;
        img, svg{
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 1;
        }
        svg{
            z-index: 2;
        }
    }
    &__info{
        flex-basis: 60%;
        .title{
            color: white;
        }
        .info{
            font-size: 20px;
            line-height: 32px;
            color: white;
            margin-top: 28px;
        }
    }
}

@media (max-width:776px) {
    .strategy{
        padding-top: 0;
        .container{
            flex-direction: column;
            gap: 0;
        }
        &__img{
            transform: translateY(-16%);
            img{
                position: relative;
            }
        }
    }
}
</style>