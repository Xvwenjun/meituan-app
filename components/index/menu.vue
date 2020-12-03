<template>
    <div class="m-menu">
            <dl class="nav"
                @mouseleave="mouseleave">
                <dt>全部分类</dt>
                <dd v-for="(item,index) in menu"
                    :key="index"
                    @mouseenter="enter">
                    <i :class="item.type"/>{{item.name}}<span class="arrow"></span>
                </dd>
            </dl>
            <div class="detail" 
                 v-if="kind"
                 @mouseenter="senter"
                 @mouseleave="sleave">
                <template v-for="(item,index) in curdetail.child">
                    <h4 :key="index">{{item.title}}</h4>
                    <span v-for="v in item.child"
                           :key="v">{{v}}</span>
                </template>
            </div>     
    </div>
</template>

<script>
export default {
    data(){
        return{
            kind:'',
            menu:[{
                type:'food',
                name:"美食",
                child:[{
                    title:'美食',
                    child:['代金券','甜食饮品','火锅','自助餐']
                }]
            },{
                type:'takeout',
                name:'外卖',
                child:[{
                    title:'外卖',
                    child:['美团外卖']
                }]

            },{
                type:"hotel",
                name:'酒店',
                child:[{
                        title:'星级酒店',
                        child:['经济型','舒适/三星','高档/四星','豪华/五星']
                }]
            }]
        }
    },
    computed:{
        curdetail:function(){
          return this.menu.filter(item=>item.type===this.kind)[0]
        }
    },
    methods:{
        enter:function(e){
          this.kind=e.target.querySelector('i').className
        },
        mouseleave:function(){
            let self = this;
            self._timer=setTimeout(() => {
                self.kind=''
            }, 150);
        },
        senter:function(){
            clearTimeout(this._timer)
        },
        sleave:function(){
            this.kind=""
        }
    }
}
</script>
<style lang="scss">

</style>