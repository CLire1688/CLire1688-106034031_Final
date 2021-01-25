<template>
  <div class='autobiography'>
    <div id="text">
      Hi, I՚m Claire, a freelance designer.<br>
      A senior student in NTHU.<br>
      My works includes websites, illustrations, and logo designs.
    </div>
  </div>
  <a id="previous" href="/" class="previous round">&#8249;</a>
</template>

<style>
  #text{
    font-family: Helvetica;
    font-size: 60px;
    font-weight:bold;
    position:absolute;
    padding: 5px;
    margin-top: 160px;
    margin-left: 39px;
    line-height: 85px;
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