<template>
  <div class="evaluate-wrapper">
        <div class="evlbox" ref="chook">
            <div class="title" >填写您的评价</div>
            <textarea class="content" type="text" @click="changeFixed" ></textarea>
            <a class="button" href="javascript:history.back(1)">确定</a>
        </div>
  </div>
</template>
<script type="ecmascript-6">
export default {
  methods: {
      //点击输入提升评论框位置
      changeFixed: function(){
        //alert(this.$refs.chook)
        this.$refs.chook.style.marginTop = "0.5625rem"
      }
  }
}
</script>
<style lang="stylus" rel="stylesheet/stylus">
    .evaluate-wrapper
        position: fixed
        top: 0
        left: 0
        width: 100%
        height: 100%
        background: rgba(0,0,0,0.5)
        z-index: 3000
        .evlbox
            margin: 3.125rem auto
            width: 9.0938rem
            height: 7.7188rem
            background: #fff  
            border-radius: 0.1875rem
            .title    
                display: block
                width: 100%
                height: 0.9375rem
                font-size: 0.4688rem
                line-height: 1.245rem
                text-indent: 0.4688rem 
            .content
                display: block
                margin: 0.3125rem auto 0 auto
                padding: 0.2188rem
                width: 7.8438rem
                height: 4.0625rem
                border: 1px solid #e0e0e0
                font-size: 0.375rem
                line-height: 1
                color: #909090
            .button
                display: block
                margin-top: 0.6406rem
                width: 100% 
                height: 1.3438rem 
                line-height: 1.3438rem 
                background: #ea6aa2
                text-align: center
                font-size: 0.5313rem
                color: #fff
                border-radius: 0 0  0.1875rem 0.1875rem 
                
</style>