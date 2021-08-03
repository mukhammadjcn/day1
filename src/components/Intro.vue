<template>
    <div class="container">
        <div class="intro">
            <div class="intro__box" v-for="(item, index) in boxes" :key="index">
                <m-info :text="item"/>
                <m-img  :img="item"/>
            </div>
            <img src="../assets/images/bg1.png" class="bgOne" alt="">
        </div>
    </div>
</template>

<script>
import MImg from './MImg.vue'
import MInfo from './MInfo.vue'
export default {
    name : "Intro",
    components: { MInfo, MImg },
    data(){
        return{
            boxes : [
                {
                    label : 'Company',
                    title : 'Company',
                    titleSpan : 'Marketing',
                    info : 'The sky was cloudless and of a deep dark blue the spectacle before us was indeed sublime.',
                    button : 'Explore',
                    img : require('@/assets/images/img1.png')
                },
                {
                    label : 'About',
                    title : 'We Build PRO Business',
                    button : 'Learn More',
                    img : require('@/assets/images/img2.png'),
                    mini : "Excited to work with customers",
                    item1 : 'The sky was cloudless and of a deep ',
                    item2 : 'Spectacle before us was indeed ',
                    item3 : 'Cloudless and of a deep dark ',
                    svg : '<svg width="24" height="22" viewBox="0 0 24 22" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M22 11C22 10.421 21.942 9.857 21.856 9.303L19.99 11.205C19.879 16.072 15.894 20 11 20C6.038 20 2 15.962 2 11C2 6.038 6.038 2 11 2C12.8 2 14.474 2.537 15.882 3.45L17.304 1.993C15.518 0.741 13.347 0 11 0C4.925 0 0 4.925 0 11C0 17.075 4.925 22 11 22C17.075 22 22 17.075 22 11ZM11.5 10.806L20.904 1.167L24 4.263L11.5 17L4.562 10.29L7.657 7.192L11.5 10.806Z" fill="#4DB282"/></svg>'
                },
                
            ]
        }
    }
    
}
</script>

<style lang="scss">
.bgOne{
        position: absolute;
        top: 0;
        right: 0;
        z-index: -1;
    }
.intro{
    padding: 64px 0;
    &__box{
        display: flex;
        justify-content: space-between;
        padding: 48px 0;
        align-items: center;
        &:nth-child(2){
            align-items: flex-start;
            flex-direction: row-reverse;
            .intro__title{
                display: none;
            }
            ul{
                margin-bottom: 38px;
                li{
                    margin-bottom: 8px;
                    font-size: 16px;
                    line-height: 32px;
                    color: #333333;
                    margin-left: 24px;
                    position: relative;
                    span{
                       svg{
                            position: absolute;
                            left: 0;
                            top: 50%;
                            transform: translate(-36px, -50%);
                       }
                    }
                }
            }
        }
        &:nth-child(1){
            .miniTitle, .title{
                display: none;
            }
        }
        .miniTitle{
            margin: 28px 0;
        }
    }
}

@media(max-width:776px){
    .intro{
        &__box{
            flex-direction: column-reverse !important;
        }
        .mInfo .intro__title{
            font-size: 56px;
            line-height: 64px;
        }
    }
    .intro__box:nth-child(2) ul{
        margin-left: 16px;
    }
}
</style>