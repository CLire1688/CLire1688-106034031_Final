<template>
  <div class='namecard'>
    <div class='wave -one'></div>
    <div class='wave -two'></div>
    <div class='wave -top'></div>

    <div class='name' style="color: white;"> CLAIRE</div>
    <div class='name' style="color: #b9965c;left: 210px;"> CHAN </div> 
    <div class='chi-name'> 詹凱淇</div>

    <div class="school">
      NTHU IEEM21        
    </div>
    <div class="e-mail">
    12cococindy@gmail.com
    </div>
  </div>
  <a id="previous" href="/" class="previous round">&#8249;</a>
</template>

<style>

  * {font-family: "Raleway", sans-serif, 微軟正黑體;
    text-decoration: none;
    }

  .namecard {
    width: 350px;
    height: 200px;
    z-index: 3;
    padding: 15px;
    margin-left: 35vw;
    margin-top: 30vh;
    position: absolute;
    background: linear-gradient(#f2f2f2, #eee);
    overflow: hidden;
    border-radius: 6px;
    box-shadow: 6px 6px 50px rgba(0, 0, 0, 0.5);
    font-weight: bold;
    transition: all 0.5s;
  }
  .namecard:after {
    content: "";
    position: absolute;
    display: block;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, #d3b990, rgba(43, 121, 124, 0) 50%, rgba(255, 255, 255, 0.5));
    transform: translate3d(0, 0, 0);
  }

  .namecard:hover {
    transform: translate3d(-0px, -12px, -12px); 
    box-shadow: 0px 0px 50px rgba(143, 142, 142, 0.774); /*滑鼠移至名片時，周圍出現白色光暈*/
  }

  .wave {
    width: 700px;
    height: 700px;
    opacity: 0.3;
    position: absolute;
    left: 0;
    background: #202C3F;
    border-radius: 40%;
    transform-origin: 50% 48%;
    transition: left 2s;
    animation: drift 3200ms infinite linear;
    margin-top: -36px;
    margin-left: -528px;
  }

  .wave.-two {
    opacity: 0.35;
    animation: drift 4000ms infinite linear;
    margin-top: -40px;
    margin-left: -430px;
  }

  .wave.-top {
    animation: drift 3500ms infinite linear;
    background-color: #d3b990; /*最上層的海浪顏色*/
    opacity: 0.25;
    margin-top: -20px;
    margin-left: -310px;
  }
  
  .name {
    top: 65px;
    left: 10%;
    position: absolute;
    display: inline-block;
    z-index: 9;
    transform: translate3d(0, 0, 0);
    color: #f2f2f2;
    letter-spacing: 6px;
    font-size: 32px;
    text-shadow: 0 1px 0 rgba(0, 0, 0, 0.1);
    
  }

  .chi-name {
    top: 115px;
    left: 11%;
    position: absolute;
    display: inline-block;
    z-index: 9;
    transform: translate3d(0, 0, 0);
    color: #f2f2f2;
    letter-spacing: 20px;
    font-size: 16px;
    font-weight: normal;
    text-shadow: 0 1px 0 rgba(0, 0, 0, 0.1);
    
  }

  .school{
    color: #46556d; 
    position: absolute;
    right: 22px;
    bottom: 35px;
    z-index: 10;
    font-size: 8px;
    font-weight: lighter;
    font-family: Arial, Helvetica, sans-serif;
  }

  .e-mail{
    color: #46556d; 
    position: absolute;
    right: 22px;
    bottom: 18px;
    z-index: 10;
    font-size: 8px;
    font-weight: lighter;
    font-family: Arial, Helvetica, sans-serif;
  }

  .background{
    height: 1000px;
    width: 100vw;
    z-index: 1;
    background-color:  #252f3f;
    position: fixed;
  }

  .circle{
    border-radius: 100%;
    position: absolute;
    border: solid 1px #d3b990e3;
    z-index: 2;
  }

  .circle1{
    width: 900px; height: 900px;
    right: 1010px;
    top: 250px;
  }

  .circle2{
    width: 1050px; height: 1050px;
    right: -350px;
    top: -450px;
  }

  .circle3{
    width: 105px; height: 105px;
    right: 1100px;
    top: 270px;
    border: solid 2px #d3b990e3;
  }
  
  /* 按鈕 */
  .previous{
    text-decoration: none;
    display: inline-block;
    /* font-size: 50px; */
    position:absolute;
    top: 0px;
    left:35px;
    color: aliceblue;
    font-size: 80px;
    font-weight: bolder;
  }

  .previous:hover {
    color: black;
  }
  .round {
    border-radius: 50%;
  }

  @keyframes drift {
    from {
    transform: rotate(0deg);
    }
    from {
    transform: rotate(360deg);
    }
  }  

</style>