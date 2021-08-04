<template>
    <div class="cases">
        <div class="container">
            <div class="cases__label">
                <h2 class="label">Portfolio</h2>
                <h2 class="title">Company Cases</h2>
                <p class="info">Apparently we had reached a great height in the atmosphere, for the sky was a dead black, and the stars had ceased to twinkle the same illusion which lifts the horizon of the sea.</p>
            </div>
            <div class="row">
                <div class="case">
                    <div class="case__img">
                        <img src="https://picsum.photos/600/600" alt="">
                        <span>01</span>
                    </div>
                    <h2 class="miniTitle">Face of Mars</h2>
                    <p class="info">Will be a rare experience</p>
                </div>
                <div class="case">
                    <div class="case__img">
                        <img src="https://picsum.photos/600/601" alt="">
                        <span>02</span>
                    </div>
                    <h2 class="miniTitle">Heavenly Bodies</h2>
                    <p class="info">Tour round the world should form</p>
                </div>
                <div class="case">
                    <div class="case__img">
                        <img src="https://picsum.photos/600/602" alt="">
                        <span>03</span>
                    </div>
                    <h2 class="miniTitle">Liberal Education</h2>
                    <p class="info">Truly it was a great journey</p>
                </div>
                <div class="case">
                    <div class="case__img">
                        <img src="https://picsum.photos/600/603" alt="">
                        <span>04</span>
                    </div>
                    <h2 class="miniTitle">Though the Gravity</h2>
                    <p class="info">Daily classes he no longer collapsed</p>
                </div>
            </div>
            <button class="contactBtn">Browse All</button>
        </div>
    </div>
</template>

<script>
export default {
    name : "Cases",
}
</script>

<style lang="scss">
.cases{
    margin-bottom: 120px;
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
    .row{
        margin: 60px 0;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 36px;
        flex-wrap: wrap;
    }
    .contactBtn{
        display: flex;
        margin: auto;
    }
}
.case{
    cursor: pointer;
    text-align: center;
    &__img{
        position: relative;
        width: 570px;
        height: 384px;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 8px;
        }
        span{
            position: absolute;
            bottom: 0;
            left: 0;
            padding: 18px 28px;
            background: #4DB282;
            border-radius: 0px 24px 0px 8px;
            font-weight: bold;
            font-size: 40px;
            line-height: 48px;
            letter-spacing: -1px;
            color: #FFFFFF;
        }
    }
    .miniTitle{
        margin-top: 24px;
    }
}

@media(max-width:776px){
    .case{
        flex-basis: 90%;
        &__img{
            width: 100%;
        }
    }
}
</style>