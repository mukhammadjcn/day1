<template>
    <div class="insights">
        <div class="container">
            <div class="insights__label">
                <h2 class="label">Latest articles</h2>
                <h2 class="title">Check Our Insights</h2>
                <p class="info">See the face of Mars, anyhow, and that will be a rare experience seems to me that a view of the heavenly bodies through a fine telescope, as well as a tour round the world.</p>
            </div>
            <div class="row">
                <div class="insight">
                    <img src="https://picsum.photos/600/610" alt="">
                    <div class="insight__details">
                        <h2 class="insight__title">What looked like a small  patch of purple grass</h2>
                        <p class="info">Truly it was a great journey, and in it I met with many, whom to know was to love.</p>
                    </div>
                </div>
            </div>
            <div class="row row2">
                <div class="insight">
                    <img src="https://picsum.photos/600/611" alt="">
                    <div class="insight__details">
                        <h2 class="miniTitle">What looked like a small  patch of purple grass</h2>
                        <p class="info">Truly it was a great journey, and in it I met with many, whom to know was to love.</p>
                    </div>
                </div>
                <div class="insight">
                    <img src="https://picsum.photos/600/612" alt="">
                    <div class="insight__details">
                        <h2 class="miniTitle">What looked like a small  patch of purple grass</h2>
                        <p class="info">Truly it was a great journey, and in it I met with many, whom to know was to love.</p>
                    </div>
                </div>
                <div class="insight">
                    <img src="https://picsum.photos/600/613" alt="">
                    <div class="insight__details">
                        <h2 class="miniTitle">What looked like a small  patch of purple grass</h2>
                        <p class="info">Truly it was a great journey, and in it I met with many, whom to know was to love.</p>
                    </div>
                </div>
            </div>

            <button class="contactBtn">Browse All</button>
        </div>
    </div>
</template>

<script>
export default {
    name : "Insights"

}
</script>

<style lang="scss">
.insights{
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
        display: flex;
        align-items: center;
        margin: 16px 0;
    }
    .row2{
        gap: 24px;
        .insight{
            flex-direction: column;
            gap: 24px;
            padding: 16px 16px 38px 16px;
            img{
                width: 100%;
                height: 240px;
            }
            .info{
                display: none;
            }
        }
    }
    .contactBtn{
        display: flex;
        margin: 64px auto 128px;
    }
}
.insight{
    display: flex;
    align-items: center;
    gap: 66px;
    padding: 16px;
    background: #FFFFFF;
    border: 1px solid #E6EDF5;
    box-sizing: border-box;
    border-radius: 8px;
    img{
        width: 554px;
        height: 336px;
        object-fit: cover;
        border-radius: 8px 8px 50px 8px;
    }
    &__title{
        font-weight: bold;
        font-size: 40px;
        line-height: 48px;
        letter-spacing: -1px;
        color: #333333;
    }
    .info{
        font-size: 20px;
        line-height: 32px;
        color: #333333;
        margin-top: 32px;
    }
}

@media (max-width:776px) {
    .row2{
        flex-direction: column;
    }
    .row .insight{
        flex-direction: column;
        img{
            width: 100%;
        }
    }
}
</style>