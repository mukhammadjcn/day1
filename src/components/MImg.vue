<template>
    <div class="mImg">
        <img :src="img.img" alt="">
    </div>
</template>

<script>
export default {
    name : "mImg",
    props : {
        img : {
            type: Object,
            default: () => {}
        }
    }
}
</script>

<style lang="scss">
.mImg{
    flex-basis: 50%;
    img{
        width: 100%;
    }
}
</style>