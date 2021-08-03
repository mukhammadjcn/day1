<template>
    <div class="contact">
        <div class="container">
            <div class="contact__wrapper">
                <div class="contact__us">
                    <h2 class="title">Kickstart Your Next Project</h2>
                    <button class="btn">Contact Us</button>
                </div>
                <p class="info">I shall see the face of Mars, anyhow, and that will be a rare experience. It seems to me that a view of the heavenly bodies through a fine telescope, as well as a tour round the world, should form a part of a liberal education.</p>
                <img class="contactBg" src="../assets/images/bg3.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : "Contact"
}
</script>

<style lang="scss">
.contact{
    position: relative;
    padding: 80px 100px;
    background: #F07566;
    border-radius: 8px;
    .contactBg{
        position: absolute;
        bottom: 0;
        left: 40%;
        transform: translateY(40%);
    }
    &__wrapper{
        display: flex;
        justify-content: space-between;
        .btn{
            background: #FBD34B;
            color: black;
            margin-top: 34px;
        }
        .info{
            flex-basis: 50%;
            color: white;
        }
    }
    &__us{
        flex-basis: 30%;
        .title{
            color: white;
        }
    }
}

@media (max-width:776px) {
    .contact__wrapper{
        flex-direction: column;
        gap: 36px;
        img{
            left: 30%;
            width: 30%;
        }
    }
    .contact{
        padding: 48px 36px;
    }
}
</style>