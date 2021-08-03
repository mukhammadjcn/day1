<template>
    <div class="mInfo">
        <h4 class="label">{{text.label}}</h4>
        <h1 class="intro__title">{{text.title}} <span>{{text.titleSpan}}</span></h1>
        <h1 class="title">{{text.title}}</h1>
        <h4 class="miniTitle">{{text.mini}}</h4>
        <p class="info">{{text.info}}</p>
        <ul>
            <li>{{text.item1}}<span v-html="text.svg"></span></li>
            <li>{{text.item2}}<span v-html="text.svg"></span></li>
            <li>{{text.item3}}<span v-html="text.svg"></span></li>
        </ul>
        <button class="btn">Explore</button>
    </div>
</template>

<script>
export default {
    name : "mInfo",
    props : {
        text : {
            type: Object,
            default: () => {}
        }
    },
    data(){
        return
    }
}
</script>

<style lang="scss">
.mInfo{
    flex-basis: 40%;
    .label{
        margin-bottom: 24px;
    }
    .intro__title{
        font-weight: bold;
        font-size: 72px;
        line-height: 80px;
        letter-spacing: -1px;
        color: #333333;
        background-repeat: no-repeat;
        background-position-y: bottom;
        padding-bottom: 16px;
        background-image: url('../assets/images/Bitmap.png');
        span{
            color: #4DB282;
        }
    }
    .info{
        margin: 24px 0;
    }
}
</style>