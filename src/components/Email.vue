<template>
    <div class="container">
            <div class="newslatter">
                <h4 class="title">Company Newsletter</h4>
                <form action="">
                    <input type="email" placeholder="Your Email">
                    <button class="btn" type="submit">Subscribe</button>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: "Newslatter"
}
</script>


<style lang="scss">
.newslatter{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 120px 0 180px;
    form{
        display: flex;
        gap: 16px;
        input{
            padding: 16px;
            background: #FFFFFF;
            border: 1px solid #DADADA;
            box-sizing: border-box;
            border-radius: 6px;
            width: 280px;
            &::placeholder{
                font-size: 16px;
                line-height: 32px;
                color: rgba(51, 51, 51, 0.496405);
            }
        }
    }
}

@media (max-width:776px){
    .newslatter{
        flex-direction: column;
        align-items: flex-start;
        gap: 36px;
        form{
            flex-direction: column;
            width: 100%;
            input{
                width: 100%;
            }
            .btn{
                width: 160px;
            }
        }
    }
}
</style>