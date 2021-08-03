<template>
    <div class="sponsors">
        <div class="container">
            <a href="/">
                <img src="../assets/images/sponsor1.png" alt="">
            </a>
            <a href="/">
                <img src="../assets/images/sponsor2.png" alt="">
            </a>
            <a href="/">
                <img src="../assets/images/sponsor3.png" alt="">
            </a>
            <a href="/">
                <img src="../assets/images/sponsor4.png" alt="">
            </a>
            <a href="/">
                <img src="../assets/images/sponsor5.png" alt="">
            </a>
            <a href="/">
                <img src="../assets/images/sponsor6.png" alt="">
            </a>
            
        </div>
    </div>
</template>

<script>
export default {
    name : "Sponsors"
}
</script>

<style lang="scss">
.sponsors{
    margin: 60px 0 120px;
    .container{
        display: flex;
        align-items: center;
        justify-content: space-around;
        flex-wrap: wrap;
        gap: 24px;
    }
}
</style>