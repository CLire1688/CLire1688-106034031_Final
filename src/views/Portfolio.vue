<template>
  <div class='portfolio'>
    <img id="car" src="https://live.staticflickr.com/65535/50872842221_7c24d568bb_c.jpg"/>
  </div>
  <a id="previous" href="/" class="previous round">&#8249;</a>
</template>

<style>
  .portfolio{
    position: absolute;
    padding-left: 270px;
    padding-top: 100px;
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
  /* .contact {
  font-family: Helvetica;
  font-size: 100px;
  font-weight:bold;
  position:absolute;
  padding: 5px;
  margin-top: 160px;
  margin-left: 39px;
  line-height: 105px;
  } */

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