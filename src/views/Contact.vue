<template>
  <div class='contact'>
    <div id="e-mail" style="display:inline;">e-mail <div style="color:white;font-size: 80px;">12cococindy@gmail.com</div></div>
    <div id="address">address <div style="color:white;font-size: 80px;"> 101 Section 2 Kuang-Fu Road</div></div>
    <div id="phone">phone <div style="color:white;font-size: 80px;"> +886-3-571-5131</div></div>
    <div id="facebook">facebook <div style="color:white;font-size: 80px;"> Claire Chan</div></div>
  </div>
  <a id="previous" href="/" class="previous round">&#8249;</a>
</template>

<style>

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
  .contact {
  font-family: Helvetica;
  font-size: 100px;
  font-weight:bold;
  position:absolute;
  padding: 5px;
  margin-top: 160px;
  margin-left: 39px;
  line-height: 105px;
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