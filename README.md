# css3-transition-animation
css3 过度和动画属性简写用法
<h2>过度</h2>

    transition: property        duration   timing-function   delay;
    过度      : 需要过度的属性  持续时间   过度方式          延时
    
    transition:all 0.35s ease-out 0.2s;
    
<h2>动画</h2>

        animation: name      duration   timing-function  delay         iteration-count     direction;
        动画     : 动画名称  持续时间   运动方式         延时时间      执行次数            是否反向
        
        animation-play-state: paused / running;
        动画播放状态        :暂停    / 运行
        div{
          width: 300px;
          height: 200px;
          background: red;
          color:#fff;
          margin: 20px auto;                  //无限循环  偶数次反向
          animation: changecolor 5s ease-out .2s infinite alternate;
        }
        @keyframes changecolor{
          0%{
            background: red;
          }
          20%{
            background:blue;
          }
          40%{
            background:orange;
          }
          60%{
            background:green;
          }
          80%{
            background:yellow;
          }
          100%{
            background: red;
          }
        }
