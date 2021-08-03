<template>
    <header class="header">
        <div class="container">
            <div class="header__left">
                <a href="/" class="logo">
                    <svg width="80" height="29" viewBox="0 0 80 29" fill="none" xmlns="http://www.w3.org/2000/svg">
                     <path d="M21.52 26.8C19.8933 27.8133 17.5467 28.32 14.48 28.32C10.5333 28.32 7.22667 27.0533 4.56 24.52C1.92 21.96 0.6 18.6533 0.6 14.6C0.6 10.4933 1.88 7.14667 4.44 4.56C7.02667 1.97333 10.3867 0.679999 14.52 0.679999C17.56 0.679999 19.8933 1.18667 21.52 2.2V8.12C19.52 6.89333 17.2933 6.28 14.84 6.28C12.68 6.28 10.8667 7.04 9.4 8.56C7.93333 10.0533 7.2 12.0667 7.2 14.6C7.2 17.08 7.93333 19.0533 9.4 20.52C10.8667 21.96 12.76 22.68 15.08 22.68C17.5867 22.68 19.7333 22.04 21.52 20.76V26.8ZM30.6913 28H24.5313L26.8513 1.04H33.6113L37.3713 10.8C38.0113 12.4267 38.5579 13.92 39.0113 15.28C39.4646 16.64 39.7579 17.6 39.8913 18.16L40.0913 18.96C40.5179 17.2 41.4513 14.48 42.8913 10.8L46.6913 1.04H53.4513L56.2513 28H50.0913L49.0913 17.56L48.5713 9.68C47.8779 11.68 46.9179 14.3067 45.6913 17.56L41.8913 27.72H38.2513L34.4913 17.56C33.8779 15.9067 33.3579 14.4267 32.9313 13.12C32.5046 11.8133 32.2246 10.9067 32.0913 10.4L31.8913 9.68C31.8913 11.5733 31.7713 14.2 31.5313 17.56L30.6913 28ZM69.1144 19.28H65.9944V28H59.8344V1.04H69.1144C72.101 1.04 74.5144 1.88 76.3544 3.56C78.221 5.24 79.1544 7.37333 79.1544 9.96C79.1544 12.92 78.181 15.2133 76.2344 16.84C74.3144 18.4667 71.941 19.28 69.1144 19.28ZM68.3944 5.96H65.9944V14.4H68.0344C71.2877 14.4 72.9144 12.92 72.9144 9.96C72.9144 7.29333 71.4077 5.96 68.3944 5.96Z" fill="#333333"/>
                    </svg>
                </a>
                <nav :class="isActive ? 'showMenu' : ''" class="nav">
                    <a href="/" class="nav__link">Service</a>
                    <a href="/" class="nav__link">Blog</a>
                    <a href="/" class="nav__link">Portfolio</a>
                    <a href="/" class="nav__link">About</a>
                    <a href="/" class="nav__link">Contact </a>   
                    <button class="cancelBtn" @click="openMenu()">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M23 20.168l-8.185-8.187 8.185-8.174-2.832-2.807-8.182 8.179-8.176-8.179-2.81 2.81 8.186 8.196-8.186 8.184 2.81 2.81 8.203-8.192 8.18 8.192z"/></svg>    
                    </button>                
                </nav>
            </div>
            <div class="header__right">
                <button class="contactBtn">Contact</button>
                <button class="hamburger" @click="openMenu()">
                    <svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M24 48C37.2548 48 48 37.2548 48 24C48 10.7452 37.2548 0 24 0C10.7452 0 0 10.7452 0 24C0 37.2548 10.7452 48 24 48Z" fill="#F07566"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M13 16C13 15.4477 13.4477 15 14 15H34C34.5523 15 35 15.4477 35 16C35 16.5523 34.5523 17 34 17H14C13.4477 17 13 16.5523 13 16ZM13 24C13 23.4477 13.4477 23 14 23H34C34.5523 23 35 23.4477 35 24C35 24.5523 34.5523 25 34 25H14C13.4477 25 13 24.5523 13 24ZM14 31C13.4477 31 13 31.4477 13 32C13 32.5523 13.4477 33 14 33H34C34.5523 33 35 32.5523 35 32C35 31.4477 34.5523 31 34 31H14Z" fill="white"/>
                    </svg>
                </button>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name : "Header",
    data(){
        return{
            isActive : false
        }
    },
    methods : {
        openMenu(){
            this.isActive =! this.isActive
        }
    }
}
</script>

<style lang="scss">
.header{
    padding: 24px 0;
    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    &__left{
        display: flex;
        align-items: center;
        gap: 36px;
    }
    .nav{
        display: flex;
        align-items: center;
        gap: 36px;
        &__link{
            font-size: 16px;
            line-height: 32px;
            color: #333333;
            transition: 0.1s ease-in;
            &:hover{
                color: #F07566;
            }
        }
    }
    &__right{
        display: flex;
        align-items: center;
        .hamburger{
            background: transparent;
            border: none;
            outline: none;
            display: none;
        }
    }
    .cancelBtn{
        display: none;
        background: none;
        border: none;
        outline: none;
    }
}
.contactBtn{
            padding: 12px 28px;
            border: 1px solid rgba(240, 117, 102, 0.236809);
            box-sizing: border-box;
            border-radius: 6px;
            font-weight: bold;
            font-size: 16px;
            line-height: 26px;
            letter-spacing: 1px;
            text-transform: uppercase;
            color: #F07566;
            background: transparent;
            outline: none;
            &:hover{
                background: #F07566;
                color: #FFFFFF;
                border: 1px solid transparent;
            }
        }

@media(max-width:776px){
    .showMenu{
        left: 0 !important;
    }
    .header{
        position: fixed;
        width: 100%;
        background: white;
        z-index: 2;
        .nav{
            left: -200%;
            position: fixed;
            display: flex;
            flex-direction: column;
            top: 0;
            width: 100vw;
            height: 100vh;
            justify-content: center;
            background: white;
            transition: 0.4s ease-out;
            z-index: 2;
            &__link{
                font-size: 36px;
                line-height: inherit;
            }
        }
        &__right{
            .contactBtn{
                display: none;
            }
            .hamburger{
                display: block;
            }
        }
        .cancelBtn{
        display: block;
        position: absolute;
        top: 36px;
        right: 44px;
        }
    }
    
}
</style>