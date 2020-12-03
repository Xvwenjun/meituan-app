<template>
   <div class="m-nav">
       <ul class="nav">
           <li class="list">
               <nuxt-link to="/my">我的美团</nuxt-link>
               <dl>
                   <dd><nuxt-link to="/order">我的订单</nuxt-link></dd>
                   <dd><nuxt-link to="/order">我的收藏</nuxt-link></dd>
                   <dd><nuxt-link to="/order">抵用券</nuxt-link></dd>
                   <dd><nuxt-link to="/order">账户设置</nuxt-link></dd>
               </dl>
           </li>
           <li class="list">
               <nuxt-link to="/mobile">手机APP</nuxt-link>
               <dl>
                   <dd><nuxt-link to="/order">登陆商家中心</nuxt-link></dd>
                   <dd><nuxt-link to="/order">我想合作</nuxt-link></dd>
                   <dd><nuxt-link to="/order">免费手机开店</nuxt-link></dd>
                   <dd><nuxt-link to="/order">商家申请合作</nuxt-link></dd>
               </dl>
           </li>
           <li class="list bd">
               <nuxt-link to="/my">商家中心</nuxt-link>
               <div class="subContainer">
                   <dl class="hotel">
                       <dt>酒店旅游</dt>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                       <dd>国际机票</dd>
                   </dl>
                   <dl class="food">
                       <dt>吃美食</dt>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                       <dd>烤鱼</dd>
                   </dl>
                   <dl class="movie">
                       <dt>看电影</dt>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                       <dd>热门</dd>
                   </dl>
                   <dl class="app">
                       <dt>手机应用</dt>
                       <dd>
                           <a href="#">
                            <img 
                            src="//s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/appicons/meituan.png"
                            alt="美团App"
                            title="美团APP">
                           </a>
                       </dd>
                       <dd>
                           <a href="#">
                            <img 
                            src="//s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/appicons/meituan.png"
                            alt="美团App"
                            title="美团APP">
                           </a>
                       </dd>
                       <dd>
                           <a href="#">
                            <img 
                            src="//s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/appicons/meituan.png"
                            alt="美团App"
                            title="美团APP">
                           </a>
                       </dd>
                       <dd>
                           <a href="#">
                            <img 
                            src="//s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/appicons/meituan.png"
                            alt="美团App"
                            title="美团APP">
                           </a>
                       </dd>
                   </dl>
               </div>
           </li>
           <li class="list bd site">
               <nuxt-link to="/my">网站导航</nuxt-link>
           </li>
           
       </ul>
    </div> 
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
</style>