# jquery轮播图插件

## 参数

** obj **         //轮播图盒子

** speed **       //动画时间

** heightAuto **  //自适应高度

** bubbleOff **   //冒泡开关

** touchOff **    //滑动开关


 
 * 轮播图插件   opt.obj 必传   opt.speed  opt.touchOff   Dom结构 div > ul > li
 * 自定义事件   需绑定在opt.obj上
 *             滑动按下自定义事件 touchStartEv    
 *             触发一次滑动移动自定义事件 touchMoveRepeatEv
 *             连续触发滑动移动自定义事件 touchMoveEv
 *             触发滑动结束自定义事件 touchEndEv
 *             动画开始前自定义事件 before
 *             动画结束自定义事件 after
 *             
 
 ***
 
## 案例
```
var $slide1 = $('#div');
$slide1.carousel({
    obj : $slide1,
    heightAuto : true
});

$slide1.on('before',function(self,obj,i){

});

$slide1.on('after',function(ev,self,newIndex){

});
```
