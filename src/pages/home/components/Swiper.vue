<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <!-- slides -->
            <swiper-slide v-for='item of swiperList' :key='item.id'>
                <img class='swiper-img' :src="item.imgUrl" />
            </swiper-slide>
          
            <!-- Optional controls -->
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
export default {
    name: 'HomeSwpier',
    data (){
        return {
            swiperOption:{
               pagination: '.swiper-pagination' ,
               loop:true
            },
            swiperList:[{
                id : '001',
                imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/201910/e7eac5a5e99e6517c61b953c0fece63b.jpg_750x200_4b701cf8.jpg'
            },{
                id : '002',
                imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/201910/95cf4225271b1e47c920473cdcec7d98.jpg_750x200_52be508b.jpg'
            },{
                id : '003',
                imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/201910/fcc952d6b479db0e7e61922f3ee70f04.jpg_750x200_c5b67f70.jpg'
            }]
        }
    }
}
</script>

<style lang="stylus" scoped>
   .wrapper >>> .swiper-pagination-bullet-active
     background #fff
   .wrapper
     overflow hidden
     width 100%
     height 0
     padding-bottom 26.66%
     background #ccc
     .swiper-img
       width 100%
</style>