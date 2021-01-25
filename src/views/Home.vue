<template>
  <div id="text">
    <div id="name" style="width:700px">
      Hi, I'm Claire Chan
    </div>
    <div class="p5Canvas"></div>
    <div id=title>
      <div id="title1"><router-link to="/autobiography">Autobiography</router-link></div>
      <div id="title2"><router-link to="/namecard">Namecard</router-link></div>
      <div id="title3"><router-link to="/portfolio">Portfolio</router-link></div>
      <div id="title4"><router-link to="/contact">Contact</router-link></div>
    </div>
  </div>
  
</template>

<script>
import P5 from 'p5';

export default {
  data() {
    return {
        p5Canvas: null,
    }
  },
  created() {
    
    const sketch = p5 => {
        let w = 300;
        let h = 100;

        // let w = window.innerWidth;
        // let h = window.innerHeight;
        p5.setup = () => {
            p5.createCanvas(1920, 1300, p5.WEBGL);
        };
        p5.draw = () => {
          p5.cursor('pointer'); 
          p5.background(255,0);

          let locX = p5.mouseX - p5.height / 2;
          let locY = p5.mouseY - p5.width / 2;
          
          p5.ambientLight(216, 192, 217, 90);
          p5.pointLight(151, 200, 229, locX, locY, 500);
          
          p5.push();   
          p5.translate(-120, -370, 0);
          p5.rotateZ(p5.frameCount * 0.01);
          p5.rotateX(p5.frameCount * 0.01);
          p5.rotateY(p5.frameCount * 0.01);
          p5.ambientMaterial(216, 192, 217);
          p5.torus(80, 20, 64, 64);
          p5.pop();

          p5.push();   
          p5.translate(-300, -150, 0);
          p5.rotateZ(p5.frameCount * 0.01);
          p5.rotateX(p5.frameCount * 0.01);
          p5.rotateY(p5.frameCount * 0.01);
          p5.ambientMaterial(180, 180, 220);
          p5.sphere(40,40);
          p5.pop();

          p5.push();   
          p5.translate(480, -620, 0);
          p5.rotateZ(p5.frameCount * 0.01);
          p5.rotateX(p5.frameCount * 0.01);
          p5.rotateY(p5.frameCount * 0.01);
          p5.ambientMaterial(180, 180, 220);
          p5.sphere(130,130,130);
          p5.pop();

          p5.push();   
          p5.translate(-720, -220, 0);
          p5.rotateZ(p5.frameCount * 0.005);
          p5.rotateX(p5.frameCount * 0.005);
          p5.rotateY(p5.frameCount * 0.005);
          p5.ambientMaterial(216, 192, 217);
          p5.box(60, 60, 60, 60);
          p5.pop();

          p5.push();   
          p5.translate(-600, -20, 0);
          p5.rotateZ(p5.frameCount * 0.008);
          p5.rotateX(p5.frameCount * 0.008);
          p5.rotateY(p5.frameCount * 0.008);
          p5.ambientMaterial(216, 192, 217);
          p5.cylinder(15, 125, 15, 55);
          p5.pop();

          p5.push();   
          p5.translate(380, -130, 0);
          p5.rotateZ(p5.frameCount * 0.01);
          p5.rotateX(p5.frameCount * 0.005);
          p5.rotateY(p5.frameCount * 0.01);
          p5.ambientMaterial(180, 180, 220);
          p5.cone(50, 70, 50);
          p5.pop();

        };

        // create methods:
        p5.changeBG = (x, y) => {
          let _x = p5.map(x, 0, w, 0, 255);
          let _y = p5.map(y, 0, h, 0, 255);
          p5.background(_x, _y, 33);
        }
    }

    this.p5Canvas = new P5(sketch, 'p5Canvas');
  },
  unmounted () {
    this.p5Canvas = null;
  },
}
</script>

<style>

#text {
  font-family: Helvetica;
  font-weight:bold;
}

#p5Canvas {
  width: 100vw;
  position: absolute;
  top: 0px;
  right: 0;
  width: 200px;
  margin: 0% !important;
}

#name {
  font-size: 50px;
  margin-block-start: 5px;
  margin-block-end: 10px;
  position: absolute;
  top: 23px;
  left: 55px;
  width: 200px;
  color:rgb(41, 117, 122);
  margin: 0%;
}

main {
  margin: 0;
  width: 30vw; 
}

#title a{
  font-size: 170px;
  color:white;
  text-decoration: none;
}

#title1 a{
  
  position: absolute;
  top: 80px;
  left: 50px;
  width: 200px;
}
#title1 a:hover {
  color:rgb(151, 151, 229);
}

#title2 a{
  position: absolute;
  top: 240px;
  left: 230px;
  width: 200px;
}
#title2 a:hover {
  color:rgb(151, 151, 229);
}

#title3 a{
  position: absolute;
  top: 400px;
  left: 420px;
  width: 200px;
}
#title3 a:hover {
  color:rgb(151, 151, 229);
}

#title4 a{
  position: absolute;
  top: 560px;
  left: 610px;
  width: 200px;  
}
#title4 a:hover {
  color:rgb(151, 151, 229);
}

</style>