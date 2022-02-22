<!DOCTYPE html>
<html>
<style>
body, html {
  height: 100%;
  margin: 0;
}

.bgimg {
  background-image: url('https://thumbs.dreamstime.com/b/website-under-construction-vector-illustration-suitable-web-landing-page-wallpaper-background-banner-book-170708888.jpg');
  height: 100%;
  background-position: center;
  background-size: cover;
  position: relative;
  color: white;
  font-family: "Courier New", Courier, monospace;
  font-size: 25px;
}

.topleft {
  position: absolute;
  top: 0;
  left: 16px;
}

.bottomleft {

font-family: "monospace";
font-size: 15px;
  position: absolute;
  bottom: 0;
  left: 20px;
}

.middle {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: black;
}

hr {
  margin: auto;
  width: 40%;
}
</style>
<body>

<div class="bgimg">
  <div class="topleft">
  </div>
  <div class="middle">
    <h1>COMING SOON</h1>
    <hr>
    <p id="time" style="font-size:30px"></p>
  </div>
  <div class="bottomleft">
    <p>All copyrights reserved to Chiheb Mabrouk 2022<br>  
    Tel:+216 29 083 421 </p>
  </div>
</div>

<script>
var countDownDate = new Date("June 5, 2022 15:37:25").getTime();

var countdownfunction = setInterval(function() {
  var now = new Date().getTime();
  var distance = countDownDate - now;

  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
  
  document.getElementById("time").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
  
  if (distance < 0) {
    clearInterval(countdownfunction);
    document.getElementById("demo").innerHTML = "EXPIRED";
  }
}, 1000);
</script>

</body>
</html>
