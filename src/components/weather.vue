<template>
  <body>
    <div class="currentCity">Саранск</div>
  <div class="imgGradus">
    <img class="weatherImgCity" src="../assets/13d.png" alt=""><div class="gradusCity">-5</div><div class="gradus">°</div>
  </div>
    <div class="weatherCity">Снег</div>
    <div class="days">По дням</div>
    
        <div class="stage_1">
            <div class="item item_1" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Сегодня</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-4° <span class="nightGradus">-7°</span></div>
            </div>

            <div class="item item_2" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Завтра</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-9° <span class="nightGradus">-6°</span></div>
            </div>

            <div class="item item_3" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Ср 10</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-8° <span class="nightGradus">-5°</span></div>
            </div>

            <div class="item item_4" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Чт 11</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-6° <span class="nightGradus">-8°</span></div>
            </div>

            <div class="item item_5" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Пт 12</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-3° <span class="nightGradus">-5°</span></div>
            </div>

            <div class="item item_6" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Сб 13</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-5° <span class="nightGradus">-9°</span></div>
            </div>

            <div class="item item_7" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Вс 14</p>
                <img class="img_1" src="../assets/13d.png" alt="Снег">
                <div class="d_1">-4° <span class="nightGradus">-7°</span></div>
            </div>

        </div>
        <div class="details">Подробнее</div>
        <hr class="h_line1"><hr class="h_line2">

        <div class="stage_2">
            <div class="item_a item__1">По ощущениям <div class="countText">-12°</div></div>
            <div class="item_a item__2">Влажность <div class="countText">68%</div></div>
            <div class="item_a item__3">Видимость <div class="countText">10 км</div></div>
            <div class="item_a item__4">Давление <div class="countText">741 мм рт.ст</div></div>
            <div class="item_a item__5">Ветер <div class="countText">
              <img class="wind" src="../assets/vector.png">9 м/с</div> </div>
            <div class="item_a item__6"></div>
        </div>

        <div class="stage_3">
            <div class="item_b item___1"><p>Восход</p>
              <img class="sunriseImg" src="../assets/sunrise.png" alt="восход"><span class="timeSun">6:47</span>
            </div>
            <div class="item_b item___2"><p>Закат</p>
              <img class="sunriseImg" src="../assets/sunset.png"  alt="закат"><span class="timeSun">17:35</span>
            </div>
        </div>
  </body>
</template>

<script>
export default {
  name: 'HelloWorld', 
  props: {
    msg: String
  }
}
</script>


<style>
* {
  margin: 0px;
  padding: 0px;
  outline: 0px;
  box-sizing: border-box;
}

body {
  font-family: 'serif';
  font-style: normal;
  color: rgb(255, 255, 255);
  background-image: url(../assets/background.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

button {
 cursor: pointer;
}
.currentCity {
  font-size: 65px;
  text-align: center;
  margin-top: 5px;
    position: absolute;
    top: 5px;
    bottom: 0px;
    left: 0px;
    right: 0px; 
}
.d_1 {
  padding-top: 10px;
}
.d1 {
  padding-bottom: 15px;

}
.imgGradus {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 75px;
  position: absolute;
    top: -700px;
    bottom: 0px;
    left: 0px;
    right: 0px; 
}
.weatherImgCity {
  margin-right: 25px;
  height: 120px;
  width: 120px;
}
.gradusCity {
  font-size: 65px;
}
.gradus {
  font-size: 50px;
}
.weatherCity {
  font-size: 35px;
  text-align: center;
  margin-top: 110px;
    position: absolute;
    top: 130px;
    bottom: 0px;
    left: 0px;
    right: 0px; 
}
.nightGradus {
  font-size: 25px;
  color: rgb(192, 191, 192);
}
.days {
  text-align: left;
  margin-left: 64px;
  font-size: 26px;
  position: absolute;
    top: 350px;
    bottom: 0px;
    left: 0px;
    right: 0px;
}
.stage_1 {
    display: flex;
    position: absolute;
    top: 400px;
    bottom: 300px;
    left: 0px;
    right: 0px;
    justify-content: space-between;
    justify-items: flex-start;
    flex-wrap: nowrap;
    border: 1px solid rgba(128, 0, 0, 0); 
    min-height: 120px;
    align-items: center;
    margin-left: 64px;
    margin-right: 64px;
    padding: 0px;
    
}
.item {
  text-align: left;
  font-size: 24px;
  padding: 15px;
  border: 1px solid rgba(0, 250, 154, 0); 
  width: 100px;
  height: 110px;
  border-radius: 10px;

}
.item_1 {
  width: 120px;
  height: 120px;
}
.img_1 {
  width: 90px;
  height: 85px;
}
.item_2 {
  width: 110px;
  height: 110px;
}
.item_3 {
  width: 110px;
  height: 110px;

}
.item_4 {
  width: 110px;
  height: 110px;
}
.item_5 {
  width: 110px;
  height: 110px;
}
.item_6 {
  width: 110px;
  height: 110px;
}
.item_7 {
  width: 110px;
  height: 110px;
}



.details {
  text-align: left;
  margin-left: 64px;
  font-size: 25px;
  position: absolute;
    top: 700px;
    bottom: 0px;
    left: 0px;
    right: 0px;
}

.countText {
  padding-top: 8px;
  font-size: 20px;

}
.h_line1 {
    display: block;
    height: 1px;
    width: 400px;
    border: 0px;
    border-top: 1px solid #ccc;
    margin-left: 64px;
    padding: 0px;
      position: absolute;
      top: 730px;
      bottom: 0px;
      left: 0px;
      right: 0px;

}
.h_line2 {
    display: block;
    height: 1px;
    width: 200px;
    border: 0px;
    border-top: 1px solid #ccc;
    margin-left: 264px;
    padding: 0px;
    position: absolute;
      top: 730px;
      bottom: 0px;
      left: 385px;
      right: 0px;
}


.stage_2 {
  display: flex;
  border: 1px solid rgba(255, 0, 0, 0); 
  min-height: 140px;
  width: 370px;
  justify-content: start;
  justify-items: flex-start;
  flex-wrap: wrap;
  margin-left: 65px;
  margin-bottom: 92px;
  text-align: left;
    position: absolute;
    top: 760px;
    bottom: 380px;
    left: 0px;
    right: 0px;
  

}
.item_a {
  border: 1px solid rgba(0, 250, 154, 0); 
  font-size: 17px;
}

.item__1 {
  width: 120px;
  height: 60px;
}

.item__2 {
  width: 120px;
  height: 60px;
}

.item__3 {
  width: 125px;
  height: 100px;
}

.item__4 {
  width: 120px;
  height: 80px;
}

.wind {
  height: 15px;
  width: 18px;
  margin-right: 10px;
}

.item__5 {
  width: 200px;
  height: 70px;
}

.item__6 {
  width: 200px;
  height: 70px;
}


.stage_3 {
  display: flex;
  border: 1px solid rgba(128, 0, 0, 0); 
  min-height: 600px;
  width: 200px;
  text-align: left;
  flex-wrap: wrap;
  margin-left: 300px;
  margin-bottom: 92px;
    position: absolute;
    top: 560px;
    bottom: 10px;
    left: 375px;
    right: 0px;

}
.item_b {
  font-size: 20px;
  align-items: flex-start;
  border: 1px solid rgba(21, 226, 147, 0);
}

.item___1 {
  width: 220px;
  height: 70px;
  margin-top: 190px;
}

.item___2 {
  width: 220px;
  height: 70px;
  margin-bottom: 10em;
}
.sunriseImg {
  margin-top: 20px;
  margin-right: 10px;
  width: 50px;
  height: 50px;
}
.timeSun {
  font-size: 19px;
}
</style>
