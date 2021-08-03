<template>
  <div class="home">
    <Header />

    <intro/>

    <service/>

    <cases/>

    <sponsors/>

    <market/>

    <strategy/>

    <team/>
    
    <testimons/>

    <contact/>

    <email />

    <insight />

    <Footer />

  </div>
</template>

<script>
import Cases from '../components/Cases.vue'
import Contact from '../components/Contact.vue'
import Email from '../components/Email.vue'
import Footer from '../components/Footer.vue'
import Header from '../components/Header.vue'
import Insight from '../components/Insight.vue'
import Intro from '../components/Intro.vue'
import Market from '../components/Market.vue'
import Service from '../components/Service.vue'
import Sponsors from '../components/Sponsors.vue'
import Strategy from '../components/Strategy.vue'
import Team from '../components/Team.vue'
import Testimons from '../components/Testimons.vue'

export default {
  name: 'Home',
  components: {
    Header,
    Intro,
    Service,
    Cases,
    Sponsors,
    Market,
    Strategy,
    Team,
    Testimons,
    Contact,
    Email,
    Insight,
    Footer
  }
} 
    
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@100;200;300;400;500;600;700;800;900&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  list-style-type: none;
  text-decoration-line: none;
  font-family: 'Work Sans', sans-serif;
}
.container{
  max-width: 1180px;
  margin: auto;
}
.title{
  font-weight: bold;
  font-size: 56px;
  line-height: 64px;
  letter-spacing: -1px;
  color: #333333;
}
.miniTitle{
  font-weight: bold;
  font-size: 24px;
  line-height: 32px;
  color: #333333;
}
.info{
  font-size: 16px;
  line-height: 32px;
  color: rgba(51, 51, 51, 0.496405);
}
.miniInfo{
  font-size: 14px;
line-height: 24px;
color: rgba(51, 51, 51, 0.496405);
}
.label{
  font-weight: bold;
  font-size: 16px;
  line-height: 32px;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #F07566;
  position: relative;
  margin-left: 24px;
  &::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 0;
    transform: translate(-24px, -50%);
    width: 12px;
    border-radius: 50%;
    height: 12px;
    background: #F07566;
  }
}
.btn{
  padding: 12px 36px;
  background: #F07566;
  border-radius: 6px;
  font-weight: bold;
  font-size: 16px;
  line-height: 26px;
  text-align: center;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #FFFFFF;
  border: 1px solid transparent;
  outline: none;
  &:hover{
    border: 1px solid rgba(240, 117, 102, 0.236809);
    color: #F07566;
    background: transparent;
  }
}

@media (max-width: 1180px) {
  .container{
    width: 94%;
  }
}
@media (max-width: 776px){
.title {
    font-size: 36px;
    line-height: 48px;
  }
}
</style>
